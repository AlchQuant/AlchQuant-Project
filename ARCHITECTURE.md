# Architecture

AlchQuant is an autonomous quantitative research and execution system
designed to discover, measure, and validate market edge. It works on
newly launched tokens, and it is chain-agnostic: the same design
applies wherever it operates, and no part of the design depends on a
single chain.

This document describes the system at a high level: what it does, how
its parts relate, and how it is kept safe. It does not describe how
the system is implemented.

## The system at a glance

The system works in a loop:

```
observe → evaluate → execute → record
```

- **Observe.** The system watches markets continuously.
- **Evaluate.** What it observes is measured against criteria
  recorded in the design. Nothing is acted on without a recorded
  basis.
- **Execute.** Actions are taken only within defined limits, and
  only in the mode the current gate allows.
- **Record.** Everything the system does, and every decision it
  makes, is recorded, so the work can be reviewed and audited.

Safety bounds the whole loop. At any point, doubt stops the system
rather than letting it proceed.

## Modes of operation

The system has three modes. A version moves between them only
through the readiness gate.

- **Paper.** The system runs against live market data without
  placing orders. Paper is where an idea first has to prove it can
  find edge without risk.
- **Shadow.** The system runs alongside the market, recording what
  it would have done. Shadow is where an idea has to prove it
  behaves as designed.
- **Live.** The system trades with real funds. No version has
  operated in this mode.

The gate between modes is the readiness gate described in the
README: it is met by evidence, not by schedule.

## Reliability

The system is built to fail closed. A failed check blocks the
version; an unknown state stops the system rather than letting it
guess. Records are kept durably, so that what the system did can
always be reconstructed and reviewed after the fact.

## Risk

Risk is managed before it is taken, not after. Exposure is bounded
by limits set in the design. An idea is tested in paper and shadow
before it is allowed near live funds, and every version is reviewed
independently before further development proceeds. The program
accepts that most ideas will fail validation; that is what
validation is for.

## Version lifecycle

Development proceeds one version at a time. Each version is
specified, implemented, tested, and independently reviewed before
the next version is undertaken. The decision record of each version
is part of the design.

## What this document does not contain

This document describes the system, not its implementation. It does
not contain source code, formulas, parameters, internal models,
decision logic, optimization or calibration methods, or entry, exit,
and position-sizing details. Those are private to the program.
