# Implementation notes

2026-10-11: Nift maintained tests show snapshot closures, native thread join, bounded-pool async functions, transferable atomics/mutexes and owner-checked values. Nested futures have forward-progress tests. Investigate callable snapshots and queue/cancellation contracts before claiming equivalence. Extra syntax can carry useful ownership/error information.
