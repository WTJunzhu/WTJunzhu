<p align="right">
  <a href="./README.zh-CN.md">简体中文</a>
</p>

# Hi, I'm ZiTong Wang 👋

> **Engineering the systems beneath the surface. Designing the games beyond the rules.**

I'm a Software Engineering undergraduate at Southeast University. I'm currently interning at Kuaishou as a backend engineer, building AI Agent infrastructure. On the other side, I design and build my own games — exploring what happens when you rethink the mechanics of play.

These two threads aren't separate. A game server is a distributed system. A coroutine scheduler is a game loop. Understanding one makes me better at the other.

---

## ⚙️ Engineering & Systems

### Industry Experience

- **Kuaishou · Algorithm Engine / Storage Engine Architecture** — Backend Development Intern (2026.05 – Present)

  Core developer of Kloong, an AI Agent long-term memory gateway built on TencentDB Agent Memory (Hindsight + Headroom). It acts as an LLM proxy layer that automatically handles memory capture, semantic recall, and context compression during user conversations — injecting persistent memory into stateless LLM calls with multi-user, multi-credential isolation.

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

<table>
<tr>
  <td><b>Languages</b></td>
  <td>Python · TypeScript · C++ · JavaScript · C# · SQL</td>
</tr>
<tr>
  <td><b>Backend & Infra</b></td>
  <td>Protobuf · RPC · WebSocket · MySQL · Redis · Docker · Linux</td>
</tr>
<tr>
  <td><b>Frontend</b></td>
  <td>React · Next.js · Vue.js</td>
</tr>
<tr>
  <td><b>AI / Agent</b></td>
  <td>LLM API Integration (OpenAI / Anthropic) · Embedding · Agent Memory · Context Compression</td>
</tr>
<tr>
  <td><b>CS Fundamentals</b></td>
  <td>Distributed Systems (Raft) · Concurrency (coroutines, epoll) · Storage Engines (skip-list) · Design Patterns</td>
</tr>
</table>

---

### 🌱 What This GitHub Is

Some repositories are exercises in engineering — understanding how a consensus algorithm works by implementing it, or what happens when a coroutine yields.

Others are exercises in imagination — asking what a card game *could* be and then building it, with real players, real servers, and real design decisions.

**The ones I'm proudest of are both.**