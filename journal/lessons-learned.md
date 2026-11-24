# Lessons learned

What the work on AlchQuant has taught us. Each lesson comes from
something that actually happened; none of them names an
implementation detail.

## Check readiness before the first run

A readiness review concluded the program was not yet ready for a
first paper run — and the gap was found by a deliberate review, not
by a failed run. We now ask whether the system is ready before
running it, and we accept "not yet" as an answer.

## Recompute every derived number

A percentage in one draft version was wrong, and it passed every
check — because the checks confirmed the sentence existed, not that
the arithmetic was right. We now recompute every derived number
from its source numbers, every time it is verified.

## Verify the delivered file, not the files on disk

A complete draft on disk is not the same as a complete file as
received: a combined delivery has arrived truncated before. We now
verify the delivered file itself, from scratch, before it is sent.

## Independent review finds what builders miss

The strongest findings of the program have come from independent
review, not from the builders' own checks. The review round is not a
formality; it is where the program is most honestly tested.
