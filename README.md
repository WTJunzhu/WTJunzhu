<p align="center">
  <a href="#english">English</a> &nbsp;|&nbsp; <a href="#chinese">简体中文</a>
</p>

<div align="center">
  <a href="https://github.com/WTJunzhu">
    <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=28&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=650&lines=Engineering+systems+beneath+the+surface;Designing+games+beyond+the+rules;Both%2C+always." alt="Typing SVG" />
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
<i>A game server is a distributed system. A coroutine scheduler is a game loop.<br/>Understanding one makes me better at the other.</i>
</p>

---

<div align="center">

| | |
|:---:|:---:|
| <img src="https://github-readme-stats.vercel.app/api?username=WTJunzhu&show_icons=true&theme=transparent&hide_border=true&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9&bg_color=0D1117" height="165" /> | <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=WTJunzhu&layout=compact&theme=transparent&hide_border=true&title_color=58A6FF&text_color=C9D1D9&bg_color=0D1117" height="165" /> |

</div>

---

<div id="english"></div>

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

<div align="center">

### 🌱 What This GitHub Is

Some repositories are exercises in **engineering** — understanding how a consensus algorithm works by implementing it, or what happens when a coroutine yields.

Others are exercises in **imagination** — asking what a card game *could* be and then building it, with real players, real servers, and real design decisions.

**The ones I'm proudest of are both.**

</div>

<br/>
<br/>
<br/>

---

<div id="chinese"></div>

<div align="center">
  <a href="https://github.com/WTJunzhu">
    <img src="https://readme-typing-svg.demolab.com?font=Noto+Sans+SC&weight=600&size=26&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=700&lines=%E5%9C%A8%E7%B3%BB%E7%BB%9F%E5%BA%95%E5%B1%82%E7%90%86%E8%A7%A3%E5%B7%A5%E7%A8%8B;%E5%9C%A8%E8%A7%84%E5%88%99%E4%B9%8B%E5%A4%96%E8%AE%BE%E8%AE%A1%E6%B8%B8%E6%88%8F;%E4%B8%A4%E8%80%85%E5%85%BC%E5%A4%87" alt="Typing SVG" />
  </a>
</div>

<h1 align="center">你好，我是王子桐 <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28"></h1>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=WTJunzhu&label=Profile%20views&color=0e75b6&style=flat" alt="访问量" />
</p>

<p align="center">
我是东南大学软件工程专业的本科生。<br/>
目前在 <b>快手</b> 担任后端开发实习生，从事 AI Agent 基础设施的建设工作。<br/>
与此同时，我设计和开发自己的游戏——重新思考游戏玩法的可能性。
</p>

<p align="center">
<i>游戏服务器就是分布式系统。协程调度器就是游戏主循环。<br/>理解其中一方，会让我更擅长另一方。</i>
</p>

---

<div align="center">

| | |
|:---:|:---:|
| <img src="https://github-readme-stats.vercel.app/api?username=WTJunzhu&show_icons=true&theme=transparent&hide_border=true&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9&bg_color=0D1117" height="165" /> | <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=WTJunzhu&layout=compact&theme=transparent&hide_border=true&title_color=58A6FF&text_color=C9D1D9&bg_color=0D1117" height="165" /> |

</div>

---

## 🛠️ 技术栈

<div align="center">

  <img src="https://skillicons.dev/icons?i=python,cpp,ts,js,cs,go,rust&theme=dark" />
  <br/>
  <img src="https://skillicons.dev/icons?i=react,vue,nextjs,nodejs,linux,docker,mysql,redis&theme=dark" />

</div>

<table align="center">
<tr>
  <td align="center"><b>AI / Agent</b></td>
  <td>LLM API（OpenAI · Anthropic）· Embedding · Agent Memory · 上下文压缩</td>
</tr>
<tr>
  <td align="center"><b>计算机基础</b></td>
  <td>分布式系统（Raft）· 并发编程（协程、epoll）· 存储引擎（跳表）· 设计模式</td>
</tr>
</table>

---

## ⚙️ 工程与系统

### 实习经历

- **快手 · 算法引擎部 / 存储引擎架构组** — 后端开发实习生（2026.05 – 至今）

  **Kloong** AI Agent 长期记忆网关核心开发。基于 TencentDB Agent Memory（Hindsight + Headroom）构建 LLM 代理层，在用户对话过程中自动完成记忆写入（capture）、语义召回（recall）与上下文压缩（compress），为无状态 LLM 调用注入持久化记忆能力，支持多用户多凭据隔离。

  从零搭建 Embedding 服务（~300 行 Python），完成容器化部署、域名注册与服务发现，配置健康检查实现故障实例自动摘除。开发 Manager 核心代理服务（~8,000 行 Python），实现 OpenAI/Anthropic 双协议兼容的 LLM 代理层，支持多用户凭据管理与请求路由。参与 TDAI Gateway（~33,000 行 TypeScript）的集成与二次开发，打通记忆读写与外部知识库的数据链路。搭建容器云基础设施（KESS + KNGX + Halo），实现服务自发现与故障自动摘除，通过 .internal 域名简化服务寻址。

### 系统项目

- **[KVStorageBaseRaft-cpp](https://github.com/WTJunzhu/KVStorageBaseRaft-cpp)** — 基于 Raft 共识算法的分布式 KV 存储数据库，C++ 从零实现。完整实现 Raft 协议：由定时线程池驱动的 Leader 选举、日志复制与提交；自研 Protobuf RPC 框架 MprRpc，自定义协议解决 TCP 粘包问题；基于跳表实现存储引擎 SkipListPro。通过客户端唯一请求 ID 与 Raft Leader 读机制保证线性一致性。

- **[coroutine-lib](https://github.com/WTJunzhu/coroutine-lib)** — 基于 C++11 的轻量级非对称 N-M 协程服务器框架。使用 `ucontext_t` + `epoll` 实现协程调度器，将 IO 事件监测与时间堆定时器统一调度；深度 Hook 阻塞系统调用（sleep、Socket IO），透明地将同步调用改造为异步非阻塞模式；基于 RAII 封装 pthread 同步原语保证线程安全。

---

## 🎮 游戏与创意项目

### 旗舰项目：[ProGyakuten](https://github.com/WTJunzhu/ProGyakuten)

一款融合 UNO 式机制与身份推理的原创多人卡牌策略游戏。在这里，我把游戏设计、服务端架构、模块配置系统和 API 设计融为一个整体——基于 TypeScript 与 Node.js 构建。它不仅是一个游戏，更是一套围绕我认同的游戏体验而设计的全栈系统。

### 多人游戏改编

- **[RivalCourts-NAISHImultiplayer](https://github.com/WTJunzhu/RivalCourts-NAISHImultiplayer)** — 经典卡牌游戏 NAISHI 的多人实时在线改编，基于 Vue 与 WebSocket 构建，支持流畅的在线对战，并完成了本地化适配。
- **[GyakutenMaker](https://github.com/WTJunzhu/GyakutenMaker)** — 基于 Ren'Py 视觉小说引擎的实验性项目，探索叙事驱动的游戏设计。

### AI 桌游实验

我通过复刻经典桌游来探索游戏 AI——不只是学习如何编码实现，更是学习如何设计和评估策略决策：

- **[SkullKing](https://github.com/WTJunzhu/SkullKing)** — 具有 AI 对手的预测类吃墩游戏
- **[TexasHoldem](https://github.com/WTJunzhu/TexasHoldem)** — 带有下注策略 AI 的德州扑克引擎

### VR 与其他

- **[VR-waste-sorting](https://github.com/WTJunzhu/VR-waste-sorting)** — 我的第一个 VR 实验：基于 Unity 与 C# 的环保教育游戏，探索沉浸式环境互动。
- **[HexTechBilliards](https://github.com/WTJunzhu/HexTechBilliards)** — 基于 TypeScript 的物理机制实验性游戏。
- **[ParkcleanVR](https://github.com/WTJunzhu/ParkcleanVR)** — 一个 VR 课程项目，探索沉浸式设计的另一种可能。

---

<div align="center">

### 🌱 这个 GitHub 是什么

一些仓库是**工程**练习——通过亲手实现来理解共识算法的工作原理，或者协程 yield 时栈上到底发生了什么。

另一些仓库是**想象力**的练习——追问一张卡牌游戏*可以*变成什么样，然后把它造出来，有真实的玩家、真实的服务器、真实的设计决策。

**而我最引以为傲的那些项目，两者兼备。**

</div>