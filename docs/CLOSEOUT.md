# Concurrency campaign closeout

Live report: https://lab.nift.dev/benchmarks/concurrency/

The frozen 64-scenario campaign is complete: 608 supported cells, 10,290 measured observations and 1,216 separate warmups. Cloud and independent local correctness/coverage audits passed. Results and interpretation are in RESULTS.md; no core changes were made.

Publication identities are recorded in CLOSEOUT.json. Accepted evidence commit 726bd44a71e6d87cd86054a4636aefd1a7c46063 is distinct from append-only lifecycle commit 768e91f9fa95c5852c9d99ad196abed763998980. All 230 accepted manifest files still match their hashes.

The report, collection and homepage pass at 1440/390/320px locally and live. Fourteen figures load, numeric column edges align, narrow tables scroll independently by keyboard and the shared favicon is unchanged. All 24 live checked files match local bytes. All 161 prior publication paths are preserved except intentional homepage/collection updates.

Labs storage guard ran before both commits: 10,459,921 tracked bytes, net addition 398,524 bytes. Largest added file is public/benchmarks/concurrency/index.html (99,089 bytes). Labs contains compact publication input and report assets, not raw samples or diagnostic corpora. Matplotlib-generated SVG path whitespace was retained; source/code checks passed.

After live verification, Linode 107886842 was deleted at 2026-10-11T10:18:14Z. Authenticated API returned 404 and CLI confirmed absence. Temporary SSH keys, known hosts, CLI configuration and cloud state were removed. The final private-material scan passed across 27,320 tracked files and expanded archive entries.

The campaign is frozen. Further Nift changes belong in the separate core workspace and should use NIFT-CORE-HANDOVER.md and its retained reproducers/profile evidence.
