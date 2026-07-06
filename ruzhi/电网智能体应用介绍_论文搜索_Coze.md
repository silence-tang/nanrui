---
AIGC:
    Label: "1"
    ContentProducer: 001191110102MACQD9K64018705
    ProduceID: 4298422798266458_0-data_volume/7658580954872594715-files/所有对话/主对话/LLM智能体在电网中的应用与论文综述.md
    ReservedCode1: ""
    ContentPropagator: 001191110102MACQD9K64028705
    PropagateID: 4298422798266458#1783221689145
    ReservedCode2: ""
---
# LLM智能体在电网中的落地应用与热门论文

> 整理日期：2026-07-05

## 目录
- [一、落地应用](#一落地应用)
  - [1.1 两大电力基座大模型](#11-两大电力基座大模型)
  - [1.2 典型落地场景](#12-典型落地场景)
  - [1.3 落地案例汇总](#13-落地案例汇总)
- [二、热门论文10篇](#二热门论文10篇)
- [参考来源](#参考来源)

---

## 一、落地应用

基于LLM的智能体已从电网试点走向规模部署，核心路径是"电力基座大模型+场景Agent+机理模型融合"，以南网"大瓦特"和国网"光明"两大基座为核心。

### 1.1 两大电力基座大模型

| 基座 | 发布方 | 发布时间 | 规模 | 覆盖范围 |
|---|---|---|---|---|
| **大瓦特** | 南方电网 | 2023-09 | 2基础+7业务域+10场景+340小模型，近800PFLOPS国产算力 | 五省区，年调用23.4亿次，已适配DeepSeek-R1本地部署 |
| **光明** | 国家电网 | 2024-12 | 千亿级多模态MoE | 总部+27家省公司，"1+N+X"架构（1基座+N专业+X插件） |

### 1.2 典型落地场景

**调度运行**：大模型+机理模型协同，实现秒级故障处置。雄安智慧调度智能体总响应时间3.2秒；国网湖南转供决策从30分钟缩至1分钟；南网"大瓦特-天璇"已在总调值班试用；广西断面监控600+厂站90+断面。

**设备运维**：目前落地最广、ROI最清晰的方向，典型模式为"端侧小模型初判+云端大模型复判+数据回流迭代"。国网×百度设备专业智能体覆盖27省市、300+地市，巡检时间减半；广西输电CV大模型识别46种缺陷、分析2000万张图；贵州160座变电站巡检从800小时压缩到2小时。2026年国网启动68亿元具身智能采购（机器狗/人形机器人），要求与光明大模型深度集成。

**营销客服**：南网智能客服处理90%客户需求；国网江苏南京将供电方案从3-5工作日缩至40分钟（准确率99.5%）；深圳"数字员工"从75名扩至119名，覆盖18业务域；营销稽查智能体"元焏"、智能审图"睿审"等专业Agent已上线。

**电力仿真**：南网"大瓦特·驭电"是全球首款电力智能仿真专业大模型，仿真速度提升1000倍、误差<1.5%，入选2024年度央企十大国之重器。

**其他方向**：南网"天权"求解器30分钟完成230万变量出清；国网浙江"碳索"助绍兴印染厂平均节能超15%；国网泰州上线全国首个无人机对话式调度智能体。

### 1.3 落地案例汇总

| # | 应用 | 落地单位 | 量化效果 |
|---|---|---|---|
| 1 | 光明电力大模型 | 国家电网+27省公司 | 供电方案编制效率提升7倍 |
| 2 | 大瓦特基座 | 南方电网五省区 | 年调用23.4亿次，客服处理90%需求 |
| 3 | 雄安智慧调度Agent | 国网雄安+南瑞 | 3.2秒总响应，处置20+异常事件 |
| 4 | 大瓦特-天璇调度 | 南网总调 | 总调值班应用，已适配DeepSeek-R1 |
| 5 | 广西断面调控Agent | 南网广西 | 监控600+厂站、90+断面 |
| 6 | 可解释AI调度 | 国网湖南 | 转供决策30min→1min |
| 7 | 大瓦特·驭电仿真 | 南网科研院 | 仿真提速1000倍，误差<1.5% |
| 8 | 设备专业智能体 | 国网+百度智能云 | 巡检时间减半，变电站2.5h→45min |
| 9 | 输电CV大模型 | 南网广西 | 识别46种缺陷，2000万张图/7万千米 |
| 10 | 换流变健康评估 | 国网山东 | 评估时间7天→分钟级 |
| 11 | 无人机对话调度 | 国网泰州 | 2秒生成工单，2026-04上线 |
| 12 | 供电方案智能生成 | 国网江苏 | 3-5工作日→40分钟，准确率99.5% |
| 13 | "元焏"营销稽查 | 深圳供电局 | AI稽查，2025-02上线 |
| 14 | "数字员工"群体 | 深圳供电局 | 119名覆盖18业务域，年办53万单 |
| 15 | 贵州大瓦特40场景 | 南网贵州 | 变电站巡检800h→2h，消纳率97% |
| 16 | "天权"求解器 | 南方电网 | 230万变量30min出清，超国际主流14% |
| 17 | "碳索"碳管理 | 国网浙江 | 绍兴21家印染厂平均节能超15% |

---

## 二、热门论文10篇

| # | 论文标题 | 作者 | 期刊/会议 | 年份 | 链接 |
|---|---|---|---|---|---|
| 1 | Large Foundation Models for Power Systems | Can Huang et al. | arXiv:2312.07044 | 2023 | https://arxiv.org/pdf/2312.07044 |
| 2 | Real-time Optimal Power Flow with Linguistic Stipulations: Integrating GPT-Agent and DRL | Z. Yan, Y. Xu (通讯) | IEEE Trans. Power Systems, 39(2):4747-4750 | 2024 | DOI: 10.1109/TPWRS.2023.3332575 |
| 3 | ElecBench: A Power Dispatch Evaluation Benchmark for LLMs | Xiyuan Zhou, Huan Zhao\*, Yan Xu\*, Junhua Zhao\* | IEEE PESGM 2025 (arXiv:2407.05365) | 2024/2025 | https://arxiv.org/abs/2407.05365 · 代码: https://github.com/xiyuan-zhou/ElecBench |
| 4 | GAIA: A Large Language Model for Advanced Power Dispatch | Yuheng Cheng, Junhua Zhao et al. | Scientific Reports 15:8925 (arXiv:2408.03847) | 2025 | https://arxiv.org/abs/2408.03847 |
| 5 | Risks of Practicing LLMs in Smart Grid: Threat Modeling and Validation | Jiangnan Li, Jinyuan Sun | arXiv:2405.06237 (v2 2024-11) | 2024 | https://arxiv.org/abs/2405.06237 |
| 6 | Enhancing LLMs for Power System Simulations: A Feedback-driven Multi-agent Framework | Mengshuo Jia, Gabriela Hug (ETH Zurich) | arXiv:2411.16707 (v3 2025-05) | 2025 | https://arxiv.org/abs/2411.16707 |
| 7 | Grid-Agent: An LLM-Powered Multi-Agent System for Power Grid Control | Yan Zhang, Deepa Kundur (多伦多大学) | arXiv:2508.05702 | 2025 | https://arxiv.org/abs/2508.05702 |
| 8 | GridMind: LLMs-Powered Agents for Power System Analysis and Operations | Hongwei Jin, Kibaek Kim (Argonne国家实验室) | arXiv:2509.02494 | 2025 | https://arxiv.org/abs/2509.02494 |
| 9 | 电力系统大模型的关键科学问题、挑战与展望 | 杜博骏, 侯庆春\*, 张宁, 康重庆 (清华/浙大) | 中国电机工程学报, 46(7):2728-2749 | 2026 | http://csee.publish.founderss.cn/rc-pub/front/front-article/download/154176802 |
| 10 | ElectriQ: A Benchmark for Assessing the Response Capability of LLMs in Power Marketing | — | arXiv:2507.22911 | 2025 | https://arxiv.org/abs/2507.22911 |

---

## 参考来源

- 科技日报：https://www.stdaily.com/web/gdxw/2024-12/19/content_276190.html
- 中国网（国网×百度设备智能体）：http://szjj.china.com.cn/m/2026-03/12/content_43370881.html
- 人民雄安网（雄安调度）：http://www.rmxiongan.com/n2/2026/0528/c383557-41593611.html
- 人民网（大瓦特·驭电）：https://app.people.cn/h5/detail/normal/6108681227600896
- 中国能源报（广西电网）：http://paper.people.com.cn/zgnyb/pad/content/202509/22/content_30106655.html
- 国家电网（光明落地）：http://www.ne.sgcc.com.cn/yw_72/202507/t20250703_6022.html
- CPEM光明半年盘点：https://www.cpem.cn/list/3/17714.html
- 深圳政府网（数字员工）：https://www.sz.gov.cn/cn/xxgk/zfxxgj/tpxw/content/mpost_12806173.html
- 传感器专家网（具身智能采购）：https://m.sensorexpert.com.cn/article/482322.html
- 北极星（大瓦特专题）：http://www.chinasmartgrid.com.cn/topic/%E5%A4%A7%E7%93%A6%E7%89%B9
- 贤集网（大瓦特+DeepSeek）：https://m.xianjichina.com/special/detail_599308.html

---

> 本内容由 Coze AI 生成，请遵循相关法律法规及《人工智能生成合成内容标识办法》使用与传播。
