---
AIGC:
    Label: "1"
    ContentProducer: 001191440300708461136T1XGW3
    ProduceID: 302a1aa5bc08e2e2805f8d884752c409_75dce229778411f1a8895254002afed2
    ReservedCode1: YMa+AWzrt1GaMDsSfYV2P/ZXGybQ43zCUpC3HowFB82EDk1n1ToGpQYKEKOFVFvDBVFE2IT0dzzzCXnRLeV89Zw4hAF3C4PmzGL4CO/zjUw2atParO3Voj/VnSVKUODResiuizj/HZrIGf9ngP+k+Z3x6FtkMSzgLhH+MhqYUujYmj9tFyg4W2iysXA=
    ContentPropagator: 001191440300708461136T1XGW3
    PropagateID: 302a1aa5bc08e2e2805f8d884752c409_75dce229778411f1a8895254002afed2
    ReservedCode2: YMa+AWzrt1GaMDsSfYV2P/ZXGybQ43zCUpC3HowFB82EDk1n1ToGpQYKEKOFVFvDBVFE2IT0dzzzCXnRLeV89Zw4hAF3C4PmzGL4CO/zjUw2atParO3Voj/VnSVKUODResiuizj/HZrIGf9ngP+k+Z3x6FtkMSzgLhH+MhqYUujYmj9tFyg4W2iysXA=
---

# 基于LLM的智能体在电网中的落地应用与前沿论文综述

> 整理时间：2026年7月

---

## 第一部分：基于LLM的智能体在电网中的落地应用

### 1. 国家电网 — 光明电力大模型

**光明电力大模型**已实现全网部署应用，是国家电网"人工智能+"战略的核心底座。

| 应用方向 | 具体落地 | 效果 |
|---|---|---|
| 电力市场服务 | 山西电力"基于AI的电力市场综合服务"场景，集成智能问答、菜单导航、交易分析、报告生成、任务执行六大功能 | 替代大量人工咨询与报告工作 |
| 配网智能诊断 | 体系化推进配网故障诊断与智能巡检 | 输电线路AI巡视覆盖率100%，缺陷识别准确率超90% |
| 战略目标 | 到2027年智能体应用普及率超80%，2030年全面建成企业级一体化智能中枢 | — |

---

### 2. 南方电网 — "大瓦特"模型体系与智能体矩阵

南方电网打造了国内电力行业最完整的"通专融合"模型体系，首批通过工信部测评，获评世界人工智能大会SAIL奖、央企十大"国之重器"。

| 应用 | 说明 | 效果 |
|---|---|---|
| **配网抢修指挥官智能体** | 融合网格-设备-地址-坐标-用户时空数据，秒级感知线路跳闸 | 故障处置从15分钟压缩至1分钟，效率提升超90%；年省投资成本超9200万元 |
| **大瓦特·天象气象大模型** | 空间分辨率1km×1km，预见期15天 | 气温预测偏差仅0.9℃，较传统方法提升20%；AI负荷预测准确率达98.78%，完全替代人工 |
| **天权电力求解器** | 国内首套自主可控电力求解器 | 支撑南方区域电力市场24h不间断运行，日均降低总发电成本7000万元 |
| **空天地一体化巡检** | 输电线路AI巡视 + 无人机 + 机器狗协同 | 日告警量从百万级降至40万级；雷击跳闸分析从1小时压缩至10分钟 |
| **119个数字员工** | 覆盖生产运维、市场营销等关键岗位 | 2025年累计完成智能巡视8.5亿次，业务办理53万单，巡检效率提升19倍 |
| **电碳算协同运营平台** | 首创电-算映射模型，以电价/绿电信号驱动算力调度 | 降低算力运营成本10%以上，实现"算随电动" |

---

### 3. 朗新科技 — 电力交易智能体

基于自研"朗新九功AI能源大模型"，打造电力交易智能体：

- 日前电价预测准确率超90%
- 价差方向判断准确率超75%
- 虚拟电厂解决方案已在江苏、浙江、广东、安徽等多省落地
- 与华为合作方案获技术认证，具备规模化商用能力

---

### 4. 蚂蚁数科 — 电力交易与新能源运营智能体

2026年SNEC大会上首次将智能体技术应用于能源行业，推出"电力交易智能体"与"新能源运营智能体"，面向虚拟电厂、分布式光伏、充电桩等海量分散资源的调度与交易场景。

---

### 5. 政策推动与行业趋势

- **2026年5月**：国家发改委等四部门印发《关于促进人工智能与能源双向赋能的行动方案》，"算电协同"首次写入国家战略
- **2026年5月**：国家能源局在深圳召开全国"人工智能+"能源现场推进会，发布51个高价值场景清单
- **2026年6月**：SNEC大会上，中国电力发展促进会专家指出"虚拟电厂是AI落地电力系统的切入口"
- 25家能源企业共同签署《开放能源领域人工智能应用高价值场景倡议书》

---

## 第二部分：10篇热门论文

### 论文 1
**Grid-Agent: An LLM-Powered Multi-Agent System for Power Grid Control**
- 作者：Yan Zhang, Ahmad Mohammad Saber, Amr Youssef, Deepa Kundur（多伦多大学）
- 发表：arXiv:2508.05702, 2025年8月
- 核心贡献：提出Grid-Agent多智能体框架，结合LLM语义推理与数值求解器，实现电网违规的自主检测与修复；在IEEE 69-bus、CIGRE MV等标准测试系统上验证了优越的违规缓解性能
- 链接：https://arxiv.org/abs/2508.05702

### 论文 2
**X-GridAgent: An LLM-Powered Agentic AI System for Assisting Power Grid Analysis**
- 作者：Yihan Wen, Xin Chen（德州农工大学）
- 发表：arXiv:2512.20789, 2025年12月
- 核心贡献：提出三层分层架构（规划-协调-执行）的智能体AI系统，集成LLM驱动的提示优化与模式自适应混合RAG，通过自然语言查询自动化复杂电网分析
- 链接：https://arxiv.org/abs/2512.20789

### 论文 3
**Operating Smart Grids by Customizing Large Model Agents**
- 作者：多机构联合
- 发表：Nature Communications Engineering, 2026年6月
- 核心贡献：系统阐述了如何定制大模型智能体以支持调度控制室任务，提出包括任务导向数据准备、电网知识接地、安全检查、分阶段部署和紧密人工监督的实用路径
- 链接：https://www.nature.com/articles/s44172-026-00709-1

### 论文 4
**Large Language Model-based Power Dispatch Agent: Framework, Application and Challenges**
- 作者：Huan Zhao, Yuheng Cheng, Dejun Xiang, Junhua Zhao, Zhaoyang Dong 等
- 发表：International Journal of Electrical Power & Energy Systems, Vol.175, 2026年2月
- 核心贡献：提出全面的LLM电力调度智能体框架（感知-规划-记忆-反思-行动五大模块），探讨了在电力调度相关任务中的能力与潜在应用
- 链接：https://doi.org/10.1016/j.ijepes.2026.111653

### 论文 5
**LLM-Based Exploitation of Edge Data in Modern Power Systems**
- 作者：Minhang Liang, Qingquan Luo, Tao Yu 等（南方电网）
- 发表：Journal of Modern Power Systems and Clean Energy (MPCE), Vol.14, 2026年1月
- 核心贡献：提出利用LLM开发电网边缘数据的三层智能架构，覆盖多模态数据融合、轻量协同推理和闭环控制，在虚拟电厂调度、智能变电站巡检和应急管理三个场景中验证
- 链接：https://doi.org/10.35833/MPCE.2025.000794

### 论文 6
**A Survey on Large Language Models Enhanced Reinforcement Learning for Smart Grid**
- 作者：张晓玉、孙秋野（东北大学），李玉帅（丹麦奥尔堡大学）等
- 发表：MPCE, DOI: 10.35833/MPCE.2025.000685, 2025年
- 核心贡献：填补了"LLM赋能强化学习在智能电网中的系统性综述"这一空白，系统梳理了方法框架-应用场景-开放挑战
- 链接：https://doi.org/10.35833/MPCE.2025.000685

### 论文 7
**A Systematic Review of Transformers and Large Language Models in the Energy Sector: Towards Agentic Digital Twins**
- 作者：Gabriel Antonesi, Tudor Cioara 等
- 发表：Applied Energy, Vol.401, 2025年12月
- 核心贡献：系统综述Transformer和LLM在能源领域的应用，涵盖预测、效率优化和智能电网管理，首次提出"Agentic Digital Twin"概念
- 链接：https://doi.org/10.1016/j.apenergy.2025.126670

### 论文 8
**Redesigning Power Grid Dispatching Automation Systems by Integrating LLMs, KGs, and AI Agents**
- 作者：Guangyi Liu, Yachen Tang, Wenxin Guo, Jian Dang
- 发表：CSEE Journal of Power and Energy Systems, Vol.11(6), 2025年11月
- 核心贡献：提出融合LLM+知识图谱+AI智能体的下一代调度自动化框架，构建"感知-认知-决策-执行"闭环智能架构
- 链接：https://doi.org/10.17775/CSEEJPES.2025.03480

### 论文 9
**Review on Application and Challenges of Large Language Models in Power Grids**
- 发表：IEEE Access / IEEE Xplore, 2025年6月
- 核心贡献：全面综述LLM在电力系统规划与运行中的应用，涵盖最优潮流、EV充电优化、故障检测、调度自动化等方向，并总结了标准化评估基准的需求
- 链接：https://ieeexplore.ieee.org/document/11037788

### 论文 10
**AutoGrid AI: 用于自主微电网管理的深度强化学习框架**
- 作者：Kenny Guo, Nicholas Eckhert, Krish Chhajer 等
- 发表：arXiv:2509.03666, 2025年9月
- 核心贡献：集成Transformer预测与PPO强化学习的自主微电网管理框架，优化可再生能源调度策略，附带开源多微电网模拟环境
- 链接：https://arxiv.org/abs/2509.03666

---

## 总结

LLM智能体在电网领域已从实验室走向生产环境，国内以**国家电网光明大模型**和**南方电网大瓦特体系**为代表，在调度、巡检、交易、客服等核心业务场景实现了规模化落地。学术界则围绕智能体架构设计（Grid-Agent、X-GridAgent）、LLM+强化学习融合、知识图谱集成、边缘数据处理等方向快速推进。政策层面，"算电协同"已上升为国家战略，AI+能源的产业化窗口正在全面打开。
*（内容由AI生成，仅供参考）*
