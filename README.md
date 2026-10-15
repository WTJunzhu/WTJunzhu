<p align="right">
  <a href="./README.zh-CN.md">简体中文</a>
</p>

<div align="center">
  <a href="https://github.com/WTJunzhu">
    <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=28&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=Engineering+the+systems+beneath+the+surface;Designing+the+games+beyond+the+rules;Both%2C+always." alt="Typing SVG" />
  </a>
</div>

<h1 align="center">Hi, I'm ZiTong Wang <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28"></h1>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=WTJunzhu&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />
</p>

<p align="center">
I'm a Software Engineering undergraduate at Southeast University.<br/>
I intern at <b>Kuaishou</b> as a backend engineer, building AI Agent infrastructure.<br/>
On the other side, I design and build my own games — rethinking the mechanics of play.
</p>

<p align="center">
<i>A game server is a distributed system. A coroutine scheduler is a game loop.<br/>Understanding one makes you better at the other.</i>
</p>

---

<div align="center">

| | |
|:---:|:---:|
| <img src="https://github-readme-stats.vercel.app/api?username=WTJunzhu&show_icons=true&theme=transparent&hide_border=true&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9&bg_color=0D1117" height="165" /> | <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=WTJunzhu&layout=compact&theme=transparent&hide_border=true&title_color=58A6FF&text_color=C9D1D9&bg_color=0D1117" height="165" /> |

</div>

---

## ⚙️ Engineering & Systems

### Industry Experience

- **Kuaishou · Algorithm Engine / Storage Engine Architecture** — Backend Development Intern (2026.05 – Present)

  Core developer of **Kloong**, an AI Agent long-term memory gateway built on TencentDB Agent Memory (Hindsight + Headroom). It acts as an LLM proxy layer that automatically handles memory capture, semantic recall, and context compression during user conversations — injecting persistent memory into stateless LLM calls with multi-user, multi-credential isolation.

  Built an Embedding service from scratch (~300 lines Python) with containerized deployment, service discovery, and health-check-based auto-failover. Developed the Manager proxy core (~8,000 lines Python), implementing an OpenAI/Anthropic dual-protocol-compatible LLM proxy layer with multi-user credential management and request routing. Participated in TDAI Gateway (~33,000 lines TypeScript) integration, bridging memory read/write with external knowledge-base data pipelines. Set up container infrastructure (KESS + KNGX + Halo) with auto-discovery, failover, and .internal domain-based service addressing.

### Systems Projects

- **[KVStorageBaseRaft-cpp](https://github.com/WTJunzhu/KVStorageBaseRaft-cpp)** — A distributed key-value store built from scratch in C++. Implements the full Raft consensus algorithm: leader election, log replication, snapshotting, and persistence — driven by a timer-thread pool. Uses a self-built RPC framework (MprRpc, based on Protobuf) with custom TCP framing and a skip-list storage engine (SkipListPro). Guarantees linearizable reads via unique client request IDs and Raft leader-read semantics.

- **[coroutine-lib](https://github.com/WTJunzhu/coroutine-lib)** — A lightweight asymmetric N-M coroutine server framework in C++11. Built on `ucontext_t` + `epoll`: integrates I/O event monitoring with a time-heap timer into a unified scheduler, deeply hooks blocking system calls (sleep, socket I/O) to transparently convert synchronous code into asynchronous, non-blocking execution. Thread-safe synchronization via RAII-wrapped pthread primitives.

---

## 🎮 Games & Creative Projects

### Flagship: [ProGyakuten](https://github.com/WTJunzhu/ProGyakuten)

An original multiplayer card-strategy game that fuses Uno-style mechanics with role-based deduction. This is where I bring everything together: game design, server architecture, module configuration systems, and API design — all built with TypeScript and Node.js. It's not just a game; it's a full-stack system designed for a gameplay experience I believe in.

### Multiplayer Adaptations

- **[RivalCourts-NAISHImultiplayer](https://github.com/WTJunzhu/RivalCourts-NAISHImultiplayer)** — A multiplayer, real-time adaptation of the classic NAISHI card game, rebuilt with Vue and WebSocket for smooth online play and localized for a new audience.
- **[GyakutenMaker](https://github.com/WTJunzhu/GyakutenMaker)** — An experimental project in the Ren'Py visual-novel engine, exploring narrative-driven game design.

### AI-Assisted Tabletop Experiments

I explore game AI by re-creating classic tabletop games — learning not just how to code them, but how to design and evaluate strategic decision-making:

- **[SkullKing](https://github.com/WTJunzhu/SkullKing)** — Trick-taking prediction game with AI opponents
- **[TexasHoldem](https://github.com/WTJunzhu/TexasHoldem)** — Poker engine with betting strategy AI

### VR & More

- **[VR-waste-sorting](https://github.com/WTJunzhu/VR-waste-sorting)** — My first VR experiment: an educational game built with Unity and C#, exploring immersive environmental awareness.
- **[HexTechBilliards](https://github.com/WTJunzhu/HexTechBilliards)** — A TypeScript game experimenting with physics-based mechanics.
- **[ParkcleanVR](https://github.com/WTJunzhu/ParkcleanVR)** — A VR university project exploring another side of immersive design.

---

## 🛠️ Tech Stack

<div align="center">

  <img src="https://skillicons.dev/icons?i=python,cpp,ts,js,cs,go,rust&theme=dark" />
  <br/>
  <img src="https://skillicons.dev/icons?i=react,vue,nextjs,nodejs,linux,docker,mysql,redis&theme=dark" />

</div>

<table align="center">
<tr>
  <td align="center"><b>AI / Agent</b></td>
  <td>LLM API (OpenAI · Anthropic) · Embedding · Agent Memory · Context Compression</td>
</tr>
<tr>
  <td align="center"><b>Fundamentals</b></td>
  <td>Distributed Systems (Raft) · Coroutines (ucontext + epoll) · Storage Engines (skip-list) · Design Patterns</td>
</tr>
</table>

---

<div align="center">

### 🌱 What This GitHub Is

Some repositories are exercises in **engineering** — understanding how a consensus algorithm works by implementing it, or what happens when a coroutine yields.

Others are exercises in **imagination** — asking what a card game *could* be and then building it, with real players, real servers, and real design decisions.

**The ones I'm proudest of are both.**

</div>