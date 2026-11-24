# AlchQuant

**Open development, not open source.**

> "An independent journey into quantitative intelligence. Research. Engineering. Continuous evolution."

AlchQuant is an autonomous quantitative research and execution system
designed to discover, measure, and validate market edge. Development is
conducted in the open: progress, decisions, failures, and lessons are
public. The source code is not public. This repository contains
documentation only.

## Overview

AlchQuant is a research program developing an autonomous trading system
for newly launched tokens. The program is conducted as an open,
documented engineering effort: every design version is specified,
implemented, tested, and independently reviewed before the next version
is undertaken.

- Status: active development since November 2026.
- Current version: draft v34.
- Live trading: none. No version has traded with real funds.

## Scope

This repository documents the program. It does not contain, describe,
or license the implementation.

### Included

- Design philosophy and objectives.
- High-level system architecture.
- Development milestones, roadmap, and changelog.
- Sanitized test statistics, experiment results, and lessons learned.
- Failures, limitations, and engineering decisions.

### Excluded

- Source code and strategy implementation.
- Formulas, parameters, internal models, and decision logic.
- Optimization and calibration methods.
- Entry, exit, and position-sizing details.
- Credentials of any kind: private keys, seed phrases, API keys, RPC
  credentials, and sensitive wallet or operational data.

## Status

As of 25 November 2026:

| Item | State |
| --- | --- |
| Current draft | v34 |
| Independent review rounds completed | 28 |
| Review verdict to date | PAPER/SHADOW ONLY (all rounds) |
| Live trading | None |
| Readiness gate for a first paper run | Not yet met |

The system has not been cleared for live trading by any review round.
The readiness gate for a first paper run remains the active work.

## Validation

- No version is considered for live operation until it has been
  demonstrated in paper and shadow runs.
- Each design version is independently reviewed before further
  development proceeds.
- Design decisions are recorded, examined, and resolved individually;
  the decision record is part of the design.
- Verification is fail-closed: a failed check blocks the version.

## Disclosure policy

Information is classified into three layers. When the classification
of an item is uncertain, it is treated as Private. Restricted
information is never published in any form.

| Layer | Contents |
| --- | --- |
| Public | Philosophy and vision, high-level architecture, milestones and changelog, sanitized test statistics, experiment results and lessons, failures, limitations, and engineering decisions. |
| Private | Source code and strategy implementation, formulas, parameters and internal models, decision logic, optimization and calibration methods, entry, exit, and position-sizing details. |
| Restricted | Private keys and seed phrases, API keys and RPC credentials, sensitive wallet configuration, authentication data and secret operational information. |

## Documentation

| Document | Contents |
| --- | --- |
| [PHILOSOPHY.md](PHILOSOPHY.md) | Purpose, principles, and objectives. |
| [ARCHITECTURE.md](ARCHITECTURE.md) | The system at a high level. |
| [ROADMAP.md](ROADMAP.md) | Milestones and direction. |
| [CHANGELOG.md](CHANGELOG.md) | Changes by version. |
| [journal/development-log.md](journal/development-log.md) | The work, in chronological order. |
| [journal/lessons-learned.md](journal/lessons-learned.md) | Findings and lessons from the work. |

## Security

If you believe restricted information has been published in this
repository, contact [@AlchQuant](https://x.com/AlchQuant) privately.
Do not repost the material.

## Disclaimer

This repository documents a research program. Nothing here is
investment advice, and nothing here is a trading signal. No part of
this documentation authorizes the use or reuse of the AlchQuant system.

## Follow the project

- X: [@AlchQuant](https://x.com/AlchQuant)

## Copyright

© 2026 AlchQuant. All rights reserved.
