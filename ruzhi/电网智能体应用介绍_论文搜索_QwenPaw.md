# 基于 LLM 的智能体在电网中的应用综述

> 整理日期：2026-07-03 | 数据来源：Google Scholar

---

## 一、已落地的应用场景

### 1. 🎛 电网调度自动化
LLM Agent 与知识图谱（KG）融合，重构传统调度系统，实现"自然语言理解 → 状态感知 → 智能决策 → 自动执行"的闭环。调度员可以用自然语言与系统交互，系统自动完成潮流计算、拓扑分析和操作建议。

- **代表工作**：Redesigning Power Grid Dispatching Automation Systems by Integrating LLMs, KGs, and AI Agents（CSEE JPES, 2025）
- **部署形态**：与现有调度自动化系统对接，LLM Agent 作为"副驾驶"辅助调度员

### 2. 🔍 实时异常检测与告警分析
利用 LLM 多智能体系统对电网运行数据进行实时监控，分层检测异常。系统采用云原生微服务架构，可实际部署。

- **代表工作**：LEMAD（Electronics, 2025）— 采用层级式 LLM 多智能体架构，在云原生环境中部署，已在实际电网基础设施数据上验证
- **代表工作**：aLLarMa（TechRxiv, 2025）— **首个被实际部署到电力系统运行环境的 LLM 应用**，处理实时告警与运行数据
- **部署形态**：云原生微服务 / 本地化部署

### 3. 📊 功率系统仿真辅助
LLM Agent 作为"仿真助手"，理解自然语言描述的任务后自动生成 Pandapower/PyPower 仿真代码，执行并对结果进行反馈修正。

- **代表工作**：Enhancing LLMs for Power System Simulations（IEEE TSG, 2025，被引 55）— 反馈驱动的多智能体仿真框架
- **部署形态**：与研究/规划部门的工作流集成，作为仿真分析的前端接口

### 4. 🧠 辅助电网分析与操作（多智能体协同）
多个 LLM Agent 分工协作，分别负责潮流计算、拓扑分析、故障排查、安全评估等任务，共同完成复杂电网分析。

- **代表工作**：GridMind（ACM SC'25 Workshops，被引 23）— LLMs-Powered Agents for Power System Analysis and Operations
- **代表工作**：X-GridAgent（arXiv, 2025，被引 13）— Judge-Agent 架构，验证智能体协助电网分析的有效性
- **部署形态**：分析平台的后端 Agent 管线

### 5. 📡 实时监测与诊断（本地部署）
将 LLM 在本地/内网部署（不在云端），避免数据外泄，对电网实时 SCADA 数据进行筛选、分析和诊断。

- **代表工作**：Power-Q（IEEE Access, 2026）— Hybrid Screener-Analyst 框架，LLM 本地部署，实现近实时的电网监测与诊断
- **部署形态**：电力公司内网本地化部署

### 6. ⚡ P2P 能源交易
LLM 增强多智能体强化学习（MARL），多个 LLM Agent 作为"交易专家"进行协商与决策，实现实时点对点电力交易。

- **代表工作**：LLM-Enhanced Multi-Agent RL with Expert Workflow for Real-Time P2P Energy Trading（IEEE TSG, 2026，被引 12）
- **部署形态**：模拟环境验证，面向未来分布式电力市场

### 7. 🌞 光伏-电动汽车接入规划
LLM 驱动多智能体对含有高比例光伏和电动汽车的配电网进行智能规划，包括容量评估、接入方案优化等。

- **代表工作**：LLM-Empowered Multi-Agent Intelligent Planning for PV-EV Penetrated Distribution Networks（Applied Energy, 2026）
- **部署形态**：配电网规划部门的辅助决策工具

### 8. 💬 可解释调度助手
LLM Agent 调用电网仿真工具（如 Grid2Op），为调度员提供可解释的操作建议，并能回答"为什么会这样建议"。

- **代表工作**：Toward an Explainable Electric Power Grid Operation Assistant Using LLMs（MIT 硕士论文, 2025）
- **部署形态**：调度员决策支持系统

### 9. 🧪 自主科研平台
以 GPT-4 等大模型为 Agent 内核，自动完成数据获取→仿真建模→结果分析→论文撰写的全流程。

- **代表工作**：RePower（Patterns / Cell, 2025，被引 26）— An LLM-Driven Autonomous Platform for Power System Data-Guided Research
- **部署形态**：科研团队使用的自动化平台

### 10. 🌱 节点碳强度计算
LLM Agent 从电力系统运行数据中自动提取信息，完成区域电力系统的节点碳强度计算与分析。

- **代表工作**：An LLM-agent-based Framework for Calculating Nodal Carbon Intensity in Regional Power Systems（Scientific Reports, 2026）
- **部署形态**：碳资产管理系统的智能化组件

---

## 二、10 篇热门论文列表

按引用数降序排列（数据截至 2026-07-03）

| # | 论文标题 | 发表处 | 年份 | 被引 | 论文链接 |
|---|---------|--------|------|------|---------|
| 1 | **Enhancing LLMs for Power System Simulations: A Feedback-Driven Multi-Agent Framework** | IEEE Trans. Smart Grid | 2025 | **55** | [IEEE](https://ieeexplore.ieee.org/abstract/document/11086353/) · [arXiv](https://arxiv.org/pdf/2411.16707) |
| 2 | **A Review of Large Language Models for Energy Systems: Applications, Challenges, and Future Prospects** | IEEE Access | 2025 | **42** | [IEEE](https://ieeexplore.ieee.org/abstract/document/11168242/) |
| 3 | **PowerGraph-LLM: Novel Power Grid Graph Embedding and Optimization with Large Language Models** | IEEE Trans. Power Syst. | 2025 | **32** | [IEEE](https://ieeexplore.ieee.org/abstract/document/11119316/) · [arXiv](https://arxiv.org/pdf/2501.07639) |
| 4 | **RePower: An LLM-Driven Autonomous Platform for Power System Data-Guided Research** | Patterns (Cell Press) | 2025 | **26** | [Cell/Patterns](https://www.cell.com/patterns/fulltext/S2666-3899(25)00059-5) |
| 5 | **GridMind: LLMs-Powered Agents for Power System Analysis and Operations** | ACM SC'25 Workshops | 2025 | **23** | [ACM](https://dl.acm.org/doi/abs/10.1145/3731599.3767409) |
| 6 | **Grid-Agent: An LLM-Powered Multi-Agent System for Power Grid Control** | arXiv | 2025 | **21** | [arXiv](https://arxiv.org/abs/2508.05702) |
| 7 | **LEMAD: LLM-Empowered Multi-Agent System for Anomaly Detection in Power Grid Services** | Electronics (MDPI) | 2025 | **20** | [MDPI](https://www.mdpi.com/2079-9292/14/15/3008) |
| 8 | **Large Language Models in Power Systems: Enhancing Control and Decision-Making** | IJISE | 2025 | **16** | [IJISE](https://ijise.ba/article/2/) |
| 9 | **X-GridAgent: An LLM-Powered Agentic AI System for Assisting Power Grid Analysis** | arXiv | 2025 | **13** | [arXiv](https://arxiv.org/abs/2512.20789) |
| 10 | **LLM-Enhanced Multi-Agent Reinforcement Learning with Expert Workflow for Real-Time P2P Energy Trading** | IEEE Trans. Smart Grid | 2026 | **12** | [IEEE](https://ieeexplore.ieee.org/abstract/document/11483246/) · [arXiv](https://arxiv.org/pdf/2507.14995) |

---

## 三、额外推荐（立足"实际部署"视角）

以下论文虽然引用数略低，但在**实际部署和工程落地**方面具有特殊参考价值：

| 论文标题 | 发表处 | 亮点 | 链接 |
|---------|--------|------|------|
| **aLLarMa: LLM-Based Application for Operational Data, Alarms and Networks** | TechRxiv, 2025 | ⭐ **首个被实际部署到电力系统运行环境的 LLM 应用**，处理真实告警流 | [TechRxiv](https://www.techrxiv.org/doi/full/10.36227/techrxiv.174284959.98439742) |
| **Power-Q: A Hybrid Screener-Analyst Framework Using LLM Agents for Real-Time Grid Monitoring and Diagnostics** | IEEE Access, 2026 | LLM **本地/内网部署**（非云端），近实时电网监测诊断 | [IEEE](https://ieeexplore.ieee.org/abstract/document/11480814/) |
| **AI Agents in Power System Operation: Application Results and Future Potentials** | IEEE PES GM, 2025 | 展示 LLM Agent 集成电网分析工具的**实际应用结果** | [IEEE](https://ieeexplore.ieee.org/abstract/document/11305547/) |
| **Redesigning Power Grid Dispatching Automation Systems by Integrating LLMs, KGs, and AI Agents** | CSEE JPES, 2025 | 与**知识图谱融合**，重构调度自动化系统 | [IEEE](https://ieeexplore.ieee.org/abstract/document/11230261/) |
| **Toward an Explainable Electric Power Grid Operation Assistant Using Large Language Models** | MIT Thesis, 2025 | LLM Agent + Grid2Op 仿真工具，实现**可解释**的调度建议 | [MIT DSpace](https://dspace.mit.edu/handle/1721.1/159085) |
| **An LLM-agent-based Framework for Calculating Nodal Carbon Intensity in Regional Power Systems** | Scientific Reports (Nature), 2026 | LLM Agent 应用于**碳追踪**场景 | [Nature](https://www.nature.com/articles/s41598-026-60053-4) |

---

## 四、总结与趋势

### 📈 当前趋势

| 维度 | 趋势 |
|------|------|
| **架构** | 🏗 **多智能体协同**是主流（分工协作 + 工具调用） |
| **部署** | 🔒 **本地/内网部署**优先（电力数据敏感，不能上公网云）|
| **工具集成** | 🔧 LLM Agent + **仿真求解器**（Pandapower/Grid2Op/PyPower）已成标配 |
| **知识融合** | 🧩 与**知识图谱**结合，解决 LLM 在电力领域的精确性问题 |
| **评估** | 📏 从概念验证走向**标准化基准**（如 PowerAgentBench-SS） |

### ⚠️ 主要挑战

1. **幻觉与精确性** — 电网运行要求绝对精确，LLM 的幻觉是核心风险
2. **实时性** — LLM 推理延迟 vs 电网毫秒级控制需求
3. **数据安全** — 电网运行数据不能出内网，需本地化部署
4. **可解释性** — 调度员需要理解 Agent 为什么做某个决策
5. **可靠性验证** — 从仿真到实际部署的鸿沟仍需弥合

---

*本文件由 Pawpaw 自动搜索整理，仅供本地参考。*
