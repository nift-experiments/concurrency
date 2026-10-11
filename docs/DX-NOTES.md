# Implementation notes

2026-10-11: Nift maintained tests show snapshot closures, native thread join, bounded-pool async functions, transferable atomics/mutexes and owner-checked values. Nested futures have forward-progress tests. Investigate callable snapshots and queue/cancellation contracts before claiming equivalence. Extra syntax can carry useful ownership/error information.

Nift pool source uses hardware_concurrency threads and has no public worker override. Blocking sleep occupies a pool worker, unlike asyncio/promises timers. Pool/job limits will be implemented explicitly. Atomics use transferable native handles; mutex protected data has checked ownership. JS has SharedArrayBuffer atomics, but no standard native mutex: mutex cells will be unavailable rather than inventing a third-party lock for a headline.

- Queue implementation exposed parser limits: nested object/index reads and writes need intermediate bindings. A failure while holding a mutex can strand sibling threads during cleanup. Rejected local attempts retain this diagnostic; no core changes. Native user error codes require the `user.` namespace; checked and normalized only at the protocol boundary.
