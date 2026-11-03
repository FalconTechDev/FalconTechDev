<img src="assets/mark.png" width="130" align="right">

I write systems software, mostly Rust. Databases, network tools, things that have to be fast and also have to be correct.

Most of this started because I wanted to know how something actually works. FalconDB exists because I wanted to see what a columnar engine looks like when you own every layer of it, down to the storage format and the encodings. It ended up faster than DuckDB on everything I measured, which surprised me more than it should have.

Every repo says how it was measured and where it loses. I've been burned enough times by my own benchmarks to be careful: a run on battery halves every engine and says nothing about it, an unpinned run on a hybrid CPU moves 40% on unchanged code, and a single reading is not a result. Quite a lot of the FalconDB README is about mistakes I made measuring it, including the ones that got published before I caught them.

### Projects

[**falcondb**](https://github.com/FalconTechDev/falcondb) — columnar analytical database in Rust. Storage, encodings, planner, executor, indices, WAL, SQL front end. Benchmarked in one process against DuckDB, DataFusion and Polars over the same Parquet file. Ahead of DuckDB and DataFusion on all 26 points I measured, behind Polars on three of them, and slower than everyone at loading Parquet.

[**netwatch**](https://github.com/FalconTechDev/netwatch) — which program is using your connection, live. Reads the kernel's own accounting, ETW on Windows and eBPF on Linux, so a process that lives for two seconds doesn't fall between two polls.

[**sotto**](https://github.com/FalconTechDev/sotto) — end-to-end encrypted secret sync for small teams. Encryption happens on your machine; the server never holds a key that could decrypt what it stores.

[**falconnet**](https://github.com/FalconTechDev/falconnet) — SQL over packet captures, with per-process attribution. Wireshark shows you frames; this answers questions.

[**synchronize**](https://github.com/FalconTechDev/synchronize) — keeps my git repos in step across machines. Syncs at login, on a timer and before shutdown. Written because I kept losing an evening's work to the laptop I wasn't sitting at.

[**help-finder**](https://github.com/FalconTechDev/help-finder) — read-only scan for questions nobody has answered yet across GitHub, Stack Overflow, HN, Habr, dev.to, Lobsters and Discourse.

### Smaller things

Each of these answers one question and stops there.

[**sql-traps**](https://github.com/FalconTechDev/sql-traps) — the same SQL on MySQL, MariaDB, PostgreSQL and SQL Server, in Docker, where the answers differ. More of them than you'd like.

[**workflow-doctor**](https://github.com/FalconTechDev/workflow-doctor) — where a GitHub Actions workflow loses its minutes: per step, retries, cache, critical path.

[**flakemap-contrib**](https://github.com/FalconTechDev/flakemap-contrib) — reruns new or changed pytest tests N times and fails on mixed results, so a flaky test gets caught in the PR that added it.

[**jest-polluter-finder**](https://github.com/FalconTechDev/jest-polluter-finder) — finds which Jest files break a victim test, by delta debugging rather than by bisecting by hand.

[**dockerfile-diff-size**](https://github.com/FalconTechDev/dockerfile-diff-size) — which instruction made the image bigger, layer by layer.

[**vk-chain**](https://github.com/FalconTechDev/vk-chain), [**mini-player**](https://github.com/FalconTechDev/mini-player), [**desktop-focus**](https://github.com/FalconTechDev/desktop-focus) — desktop apps for Windows. A friend-of-a-friend path finder for VK, floating always-on-top video windows, and a way to hide every desktop icon except the ones you want.

### Elsewhere

I send patches to projects I use. Some of the forks here are that, not abandoned copies.

If something here is wrong or doesn't build on your machine, open an issue. I'd rather know.
