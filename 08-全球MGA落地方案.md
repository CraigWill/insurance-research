# 08 · 全球 MGA 落地方案（真 MGA / Delegated Authority）

> 场景：你面向**全球市场**做 MGA，因此可以使用真正的"承保笔"（delegated underwriting authority）。本文是 [07 号文件](./07-MGA商业模式.md)的实操延伸。
> 免责：不构成法律/监管意见。各辖区 MGA 登记与授权规则差异大，落地前须由当地保险监管律师与 capacity 提供方共同确认。

---

## 0. 先纠正一个关键前提：寿险 MGA ≠ 财险 MGA

你同时提到"筹建寿险"和"做 MGA"，这两件事在全球市场里属于**两个不同的世界**，先分清楚：

| | 财险 / 特殊险 MGA（P&C / Specialty） | 寿险 / 健康险分销中介 |
|---|---|---|
| 全球 MGA 市场占比 | **95%+**（MGA 这个业态基本是为 P&C 生的） | 很小，且形态不同 |
| 典型称呼 | MGA / MGU / Coverholder | 美国：**IMO / FMO / BGA / IMO**；英国：寿险很少用 delegated authority |
| 是否真有"承保笔" | ✅ 是（bind 风险、出单、部分理赔） | ⚠️ 有限：可代填件、简易核保，但**寿险核保决定权通常仍在保险公司**（涉及体检、财务核保、长期负债） |
| 核心资本市场 | 伦敦劳合社（Lloyd's）、百慕大、美国 E&S 市场 | 美国寿险分销层级（carrier→IMO→agency→agent） |
| MGA 收入灵魂 | 佣金 + **利润分成（profit commission）** | 佣金层级（override）+ 奖金，利润分成罕见 |

**结论（重要）**：
- 如果你说的"寿险"是指**筹建持牌寿险公司**（重资本主体），那走 [09 号文件](./09-寿险公司筹建首年计划.md)（本次同时产出）。
- 如果你想做的是**寿险方向的 MGA**，全球范围内最贴近的形态是**美国的 IMO/BGA 模式**，而不是伦敦式 P&C MGA——本文第 6 节专门讲。
- 如果你想做**真正意义上的、带承保笔和利润分成的 MGA**，那几乎必然落在 **P&C / 特殊险**，capacity 主要来自 Lloyd's 和百慕大——本文第 1–5 节。

下面两条线都给你。

---

## 1. 全球真 MGA 的产业结构（P&C / Specialty）

```
资本 / 投资人 (ILS基金、PE、再保人自有资本)
      │  提供承保能力，承担最终赔付
      ▼
承保能力提供方 Capacity Provider
  ├─ Lloyd's 辛迪加 (通过 Coverholder 授权)
  ├─ 百慕大 / 欧洲 / 美国的保险公司或再保人
  └─ Fronting Carrier (纯出借牌照+资产负债表，自身几乎全部再保出去)
      │  【Binding Authority / Delegated Authority Agreement】授予承保笔
      ▼
┌──────────────────── MGA / MGU (你) ────────────────────┐
│ Underwriting: 在授权范围内选择风险、定价、bind、出单     │
│ Distribution: 对接经纪/代理/直客                         │
│ Claims: 若获 delegated claims authority，可核赔(常配 TPA)│
│ Data & Ops: 定价模型、系统、bordereaux 报送             │
└──────────────────────────────────────────────────────────┘
      │
      ▼
Retail / Wholesale Brokers → 终端客户
```

**三种 capacity 来源的取舍：**

| 来源 | 优点 | 缺点 | 适合 |
|---|---|---|---|
| **Lloyd's Coverholder** | 全球牌照网络、品牌信用、评级 | 审批严、合规重（Coverholder 审批 + 年度审计） | 特殊险、国际业务 |
| **Fronting Carrier**（如美国有大量专业 fronting 公司） | 灵活、快、可对接 ILS/再保资本 | 需自带再保支持；fronting fee | 有独立 capacity 来源的 MGA |
| **传统保险公司直接授权** | 关系深、稳定 | 单一依赖风险 | 单一细分市场深耕 |

---

## 2. 选辖区：MGA 主体注册在哪

MGA 本身注册地 ≠ 承保业务覆盖地。选址看**监管成熟度、capacity 接近度、税务、人才**。

| 辖区 | 定位 | 适合 | 关键点 |
|---|---|---|---|
| **英国（伦敦）** | 全球 MGA 中心、Lloyd's 所在地 | 特殊险、国际业务、想接 Lloyd's capacity | 受 FCA 监管；MGA 需授权或作为 Appointed Representative；Coverholder 审批 |
| **美国（各州）** | 全球最大 MGA/E&S 市场 | 面向美国市场、寿险 IMO | MGA 需在州保险厅登记（多为 MGA/MGU license）；E&S 剩余市场空间大 |
| **百慕大** | 再保/ILS 资本中心 | 靠近 capacity、大额特殊险 | 监管成熟（BMA）、税务友好 |
| **新加坡** | 亚洲特殊险枢纽 | 面向亚太 | MAS 监管；亚洲 MGA 生态成长中 |
| **迪拜（DIFC/ADGM）** | 中东枢纽 | 面向中东非 | 独立金融特区监管 |
| **欧盟（如马耳他、爱尔兰、卢森堡）** | 欧盟护照 | 面向欧盟全境 | 一地授权、全欧展业（passporting） |

**决策逻辑**：先定"承保哪类风险、capacity 从哪来、客户在哪"，再倒推注册地。多数国际特殊险 MGA 选**英国或美国 + 百慕大 capacity**的组合。

---

## 3. 授权协议（Delegated Authority / Binding Authority）关键条款清单

这是 MGA 的"公司宪法"——你的承保笔有多大、边界在哪，全在这份协议里。谈判时逐条盯：

| 条款 | 内容 | MGA 视角要点 |
|---|---|---|
| **Scope of Authority（授权范围）** | 可承保的险种、地域、业务类别 | 越清晰越好；争取覆盖你的目标细分 |
| **Underwriting Guidelines（核保指引）** | 可接受风险、费率、限额、除外 | 这是你的"操作手册"；争取定价自主度 |
| **Limits（限额）** | 单一风险限额、单一事故限额、**aggregate（年度累计限额）** | aggregate 决定你一年能写多少；太低会限制增长 |
| **Referral（上报事项）** | 超出授权必须上报 carrier 的情形 | 越少越灵活，但 carrier 会要求关键风险上报 |
| **Premium Handling（保费处理）** | 保费收取、受托账户（fiduciary/IBA account）、结算周期 | 明确资金流与留存权 |
| **Commission & Profit Commission** | 基础佣金率 + **利润分成公式与门槛（loss ratio 阈值）** | ★收入核心；谈 loss ratio 计算口径、IBNR 处理、多年平滑 |
| **Bordereaux Reporting** | 承保/理赔台账报送频率与格式（如月度 premium & claims bordereaux） | 数据报送是 MGA 的合规命脉，系统必须支持 |
| **Claims Authority（理赔授权）** | 是否授权核赔、限额、TPA 安排 | 有理赔授权=更完整的价值链，但责任更大 |
| **Audit Rights（审计权）** | carrier 对 MGA 的现场/远程审计 | 必然有；准备好 SOC/流程文档 |
| **Term & Termination（期限与终止）** | 合约期、终止条件、**run-off（在保业务的后续处理）** | ★命门条款：被终止后在保保单如何续、佣金如何延续 |
| **Run-off & Novation** | 授权终止后存量保单的管理与转移 | 保护你的账册价值 |
| **Errors & Omissions / Indemnity** | 责任划分、E&O 保险要求 | MGA 必须自购 E&O 险 |
| **Data Ownership** | 承保与客户数据归属 | ★争取数据共有/可用权——数据是你的核心资产 |
| **Regulatory Compliance** | 反洗钱、制裁筛查、消费者保护、当地登记 | 明确各自责任边界 |

> **谈判优先级**：① 利润分成公式与 loss ratio 口径 ② aggregate 限额（增长空间）③ run-off/终止条款（账册价值保护）④ 数据归属。这四条决定你的 MGA 值不值钱。

---

## 4. Capacity 谈判：怎么让保险公司/再保人把"笔"交给你

capacity 提供方凭什么信任一个新 MGA？你要拿出这四样：

| 要素 | 提供什么证据 |
|---|---|
| **1. Underwriting alpha（定价优势）** | 目标细分的历史 loss ratio 数据、你的定价模型、为什么你比市场更准（独家数据/领域专长） |
| **2. Distribution（分销能力）** | 已有的经纪关系/流量/客户管道，预期保费规模（GWP ramp-up 曲线） |
| **3. Team（团队资质）** | 核保负责人的资历（capacity 方最看重"谁在 bind"）、精算、运营、合规 |
| **4. Governance & Systems（治理与系统）** | 核保指引、bordereaux 报送能力、合规框架、E&O 保险、审计准备 |

**谈判路径（现实版）**：
```
① 用咨询/顾问身份或再保经纪协助，先拿到目标细分的历史数据，验证 loss ratio 假设
② 做一份 business plan：细分市场规模 + 预期损失率 + 分销计划 + 3年 GWP 预测
③ 通过再保经纪（如 specialist broker）撮合 capacity（他们认识所有 carrier/syndicate）
④ 争取"小额度试点授权"（limited binder）→ 用 6–12 个月真实账册数据
⑤ 账册盈利 → 扩大 aggregate 限额 + 谈更高利润分成 + 增加 capacity panel
```

> **核心洞察**：新 MGA 拿 capacity 最快的路径是**通过专业再保经纪**（reinsurance broker / wholesale broker），他们是 MGA 和 capacity 之间的撮合方，也是你后续多元化 capacity 的通道。不要试图自己一家家敲保险公司的门。

---

## 5. 全球 P&C MGA 的启动清单与经济模型

### 5.1 12–18 个月启动清单
```
月 0-3   选细分市场 + 验证定价优势(拿历史数据) + 确定注册辖区
月 3-6   注册主体 + 监管登记(FCA授权/州MGA牌照/Coverholder申请)
         + 组建核心团队(核保负责人是关键先生)
月 4-9   通过再保经纪撮合 capacity + 谈 Binding Authority
月 6-10  建系统(核保/出单/bordereaux/理赔) + 合规框架 + 购 E&O
月 9-12  小额度试点授权上线 + 首批业务
月 12-18 用账册数据扩大授权 + 多元化 capacity + 启动利润分成
```

### 5.2 单位经济学
```
年收入 = GWP × (基础佣金率 + 管理费率) + 利润分成
利润分成 = max(0, GWP × (1 − loss ratio − 费用 − 再保成本)) × 分成比例%

利润杠杆：loss ratio 每降低 1%，利润分成显著放大
→ MGA 的估值 = 账册质量(稳定低 loss ratio) × capacity 稳定性 × 数据资产
```
**退出**：优质 MGA 的账册 + 团队 + 数据是活跃的收购标的（保险公司、再保人、PE、MGA 平台整合方都在买）。这是比自建保险公司**流动性好得多**的变现路径。

---

## 6. 如果你要做的是"寿险 MGA"：美国 IMO / BGA 模式

寿险没有伦敦式的 P&C binding authority 生态。全球范围内，寿险分销的"MGA 等价物"主要在**美国**：

```
寿险公司 (Carrier)
   │  提供产品、承保(核保决定权仍在 carrier)、佣金层级(commission schedule + override)
   ▼
IMO / FMO (Independent/Field Marketing Organization) ← 你可以做这个
   │  聚合大量代理/agency，提供培训、案例支持、简易核保前置、技术平台
   │  从 carrier 拿高 override，向下分配佣金，赚层级差 + 奖金 + 产品津贴
   ▼
Agency / BGA (Brokerage General Agency)
   ▼
独立寿险代理人 / 顾问 → 终端客户
```

| 模式 | 你做什么 | 收入 | 是否有"承保笔" |
|---|---|---|---|
| **IMO / FMO** | 聚合并赋能大量代理、对接多家 carrier、提供技术与案例支持、争取高 override | 佣金 override 差 + carrier 奖金/津贴 + 平台费 | ❌（核保在 carrier；但可做简易核保/加速核保前置） |
| **BGA** | 区域性总代理，服务独立代理的个案（尤其大额寿险、医疗核保件） | 佣金 override | ❌ |
| **寿险科技 / InsurTech MGA** | 数字化投保、自动核保引擎、直销平台，与 carrier 深度合作 | 平台费 + 佣金 + 数据 | ⚠️ 部分简易/加速核保可被授权，复杂件仍回 carrier |

**寿险 MGA 的现实要点：**
- 寿险的核保涉及**体检、财务核保、长期负债定价**，carrier 极少下放完整核保权 → 不要指望寿险版"承保笔"。
- 寿险 MGA 的价值在**分销规模 + 代理赋能 + 数字化核保体验**，靠 **override 层级 + 规模奖金**赚钱。
- 增长快的是 **InsurTech 型寿险 MGA/平台**：用技术做加速核保（accelerated underwriting，免体检）、数字化投保、直销，与 carrier 分工。
- 若目标是**利润分成型、带承保笔的真 MGA**，请务必转向 **P&C/特殊险**（第 1–5 节）——寿险给不了这个结构。

---

## 7. 给你的 MGA 决策建议

| 你的真实目标 | 推荐形态 | capacity/carrier 来源 | 注册地 |
|---|---|---|---|
| 要"承保笔 + 利润分成"的真 MGA | **P&C / 特殊险 MGA** | Lloyd's / 百慕大 / fronting carrier | 英国 或 美国+百慕大 |
| 寿险方向、要规模化分销 | **美国 IMO / FMO** 或 **InsurTech 寿险平台** | 多家美国寿险 carrier | 美国 |
| 亚太市场 | P&C MGA 或数字化分销 | 亚洲 carrier / 新加坡再保 | 新加坡 |

> **一句话**：真正意义上"像迷你保险公司、能分承保利润"的 MGA，几乎都在财险/特殊险；如果你坚持寿险，全球范围最现实的是**美国 IMO 模式**，赚的是佣金层级和分销规模，不是承保利润分成。

---

## 8. MGA 路线与"筹建寿险公司"的关系

你同时在看这两条，其实可以设计成**一条进化路径**：

```
阶段1: 做 MGA(P&C特殊险) 或 寿险IMO
        → 积累: 细分市场专长 + 数据 + 分销 + 承保/损失率证据
        ↓
阶段2: 账册盈利 + 数据资产成熟
        → 议价权提升，收入稳定，验证了"你能选好风险/卖得动"
        ↓
阶段3: 用账册数据与团队反向申请/收购保险牌照
        → 从"轻能力"升级为"重主体"，把利润分成变成完整承保利润
```

**这是全球保险业最经典的进化路线**：先做 MGA 证明定价与分销能力，再拿牌照吃下完整价值链。比一上来就砸资本筹建寿险公司**风险低得多、验证快得多**。

如果你确定终局是寿险公司，建议顺序：**先做美国寿险 IMO / InsurTech 分销 → 跑通获客与核保数据 → 再谈筹建/收购寿险牌照**（见 [09 号文件](./09-寿险公司筹建首年计划.md)）。
