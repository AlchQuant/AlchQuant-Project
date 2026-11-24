# Roadmap

This document states where the AlchQuant program is headed, and what
must happen before each step. It is a sequence of gates, not a
schedule: a phase begins when the evidence for it exists, not when a
date arrives.

## How to read this roadmap

Each phase has a status. Statuses change only when a design version
is finished, verified, and reviewed.

- **Done** — the phase is complete.
- **In progress** — the program is working in this phase now.
- **Not yet** — the phase cannot begin until the gate before it is met.

## Phases

### 1. Design and review — In progress

Versions are specified, implemented, tested, and independently
reviewed, one at a time. The program is in this phase now: current
draft v34, 28 review rounds completed, every verdict to date
PAPER/SHADOW ONLY.

### 2. First paper run — Not yet

The system runs against live market data without placing orders.
This phase begins only when the readiness gate for a first paper run
is met. The gate is not yet met.

### 3. Shadow operation — Not yet

The system runs alongside the market, recording what it would have
done. This phase begins only after paper operation has shown the
system behaves as designed.

### 4. Live trading — Not yet

The system trades with real funds. This phase begins only when the
evidence from paper and shadow operation warrants it. No version has
operated in this mode.

## What will not happen

- No version moves to live trading before the readiness gate is met.
- No date is promised for any phase. The program moves at the speed
  of its evidence.
