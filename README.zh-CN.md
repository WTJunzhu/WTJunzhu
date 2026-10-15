<p align="right">
  <a href="./README.md">English</a>
</p>

# 你好，我是王子桐 👋

> **在系统底层理解工程。在规则之外设计游戏。**

我是东南大学软件工程专业的本科生，目前正在快手担任后端开发实习生，从事 AI Agent 基础设施的建设工作。与此同时，我设计和开发自己的游戏——探索重新思考玩法机制后，游戏可以变成什么样。

这两条线索从未分离。游戏服务器就是分布式系统，协程调度器就是游戏主循环。理解其中一方，会让我更擅长另一方。

---

## ⚙️ 工程与系统

### 实习经历

- **快手 · 算法引擎部 / 存储引擎架构组** — 后端开发实习生（2026.05 – 至今）

  Kloong AI Agent 长期记忆网关核心开发。基于 TencentDB Agent Memory（Hindsight + Headroom）构建 LLM 代理层，在用户对话过程中自动完成记忆写入（capture）、语义召回（recall）与上下文压缩（compress），为无状态 LLM 调用注入持久化记忆能力，支持多用户多凭据隔离。

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

## 🛠️ 技术栈

<table>
<tr>
  <td><b>编程语言</b></td>
  <td>Python · TypeScript · C++ · JavaScript · C# · SQL</td>
</tr>
<tr>
  <td><b>后端 & 基础设施</b></td>
  <td>Protobuf · RPC · WebSocket · MySQL · Redis · Docker · Linux</td>
</tr>
<tr>
  <td><b>前端</b></td>
  <td>React · Next.js · Vue.js</td>
</tr>
<tr>
  <td><b>AI / Agent</b></td>
  <td>LLM API 集成（OpenAI / Anthropic）· Embedding · Agent Memory · 上下文压缩</td>
</tr>
<tr>
  <td><b>计算机基础</b></td>
  <td>分布式系统（Raft）· 并发编程（协程、epoll）· 存储引擎（跳表）· 设计模式</td>
</tr>
</table>

---

### 🌱 这个 GitHub 是什么

一些仓库是工程练习——通过亲手实现来理解共识算法的工作原理，或者协程 yield 时栈上到底发生了什么。

另一些仓库是想象力的练习——追问一张卡牌游戏*可以*变成什么样，然后把它造出来，有真实的玩家、真实的服务器、真实的设计决策。

**而我最引以为傲的那些项目，两者兼备。**