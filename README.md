<img src="assets/hero.png" width="100%">

Most of this started because I wanted to know how something actually works, down to the layer nobody looks at.

Every repo says how it was measured and where it loses. I've been burned enough times by my own benchmarks to be careful about that.

### What I'm building

<img src="assets/mini-falcondb.png" height="20" align="top">&nbsp; **[falcondb](https://github.com/FalconTechDev/falcondb)** &nbsp;·&nbsp; `Rust`<br>
A columnar analytical database, written from the storage format up. Faster than DuckDB and DataFusion on all 26 points I measured, and slower than everyone at loading Parquet.

**[netwatch](https://github.com/FalconTechDev/netwatch)** &nbsp;·&nbsp; `Rust`<br>
Which program is using your connection, live. Reads the kernel's own accounting instead of polling, so a process that lives two seconds isn't missed.

**[falconnet](https://github.com/FalconTechDev/falconnet)** &nbsp;·&nbsp; `Rust`<br>
SQL over packet captures. Wireshark shows you frames; this answers questions.

<img src="https://raw.githubusercontent.com/FalconTechDev/synchronize/main/docs/logo.png" height="20" align="top">&nbsp; **[synchronize](https://github.com/FalconTechDev/synchronize)** &nbsp;·&nbsp; `Go`<br>
Keeps my git repos in step across machines. Written after losing an evening's work to the laptop I wasn't sitting at.

**[help-finder](https://github.com/FalconTechDev/help-finder)** &nbsp;·&nbsp; `Python`<br>
Finds questions nobody has answered yet, across seven sites.

### Smaller, sharper

Each answers one question and stops.

- **[sql-traps](https://github.com/FalconTechDev/sql-traps)** — the same SQL on four databases, where the answers differ. More often than you'd like.
- **[workflow-doctor](https://github.com/FalconTechDev/workflow-doctor)** — where a GitHub Actions run loses its minutes.
- **[flakemap-contrib](https://github.com/FalconTechDev/flakemap-contrib)** — catches a flaky test in the PR that added it.
- **[jest-polluter-finder](https://github.com/FalconTechDev/jest-polluter-finder)** — which Jest file breaks the test you're staring at.
- **[dockerfile-diff-size](https://github.com/FalconTechDev/dockerfile-diff-size)** — which instruction made the image bigger.

### On the desktop

- **[vk-chain](https://github.com/FalconTechDev/vk-chain)** — how you know someone on VK, in hops.
- **[mini-player](https://github.com/FalconTechDev/mini-player)** — floating video windows that stay on top.
- **[desktop-focus](https://github.com/FalconTechDev/desktop-focus)** — hides every icon except the ones you want.

---

Some of the forks here are patches to projects I use, not abandoned copies — [sotto](https://github.com/getsotto/sotto) among them.<br>
If something doesn't build on your machine, open an issue. I'd rather know.
