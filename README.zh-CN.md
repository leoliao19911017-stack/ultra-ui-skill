# Ultra UI Skill · 超级 UI 技能

把 AI 生成的「模板味」界面，扭转向有辨识度、可观察、面向生产的设计方向的一套工作流。

**English: [README.md](README.md)**

> 一个 Claude Code / Codex 技能。它指导**设计判断**，不替代用户研究、无障碍测试与生产验证。
> 框架无关、模型无关、厂商无关。

---

## 它解决什么问题

AI 生成界面有三个通病：

1. **一眼 AI 味** —— 紫色渐变、发光圆角、彩色胶囊标签、无意义的 emoji 图标
2. **千篇一律** —— 每个项目都从空白页开始，最后长得都一样
3. **说不清好在哪** —— 主观的「好看」无法转成可执行的设计决策

本技能把这三件事分别对应到：**反 AI 味清单**、**10 套命名风格预设**、**可观察的设计简报**。

---

## 核心内容

| 能力 | 说明 |
|---|---|
| **风格预设** | 10 套命名风格 + 6 组命名组合，不用每次从空白页开始 |
| **风格转译** | 把主观审美转成「可观察的简报」：具体决策 + 明确禁止项 |
| **视觉评审** | 用独立的视觉评审员看截图/原型，把「肉眼可见的差距」和「未验证的风险」分开 |
| **收敛修订** | 限定最大轮数、停止条件、继续迭代的明确授权，避免无限改 |
| **去 AI 味** | 移除常见 AI 痕迹，再检查真实内容、状态、无障碍、响应式、性能与打磨度 |

---

## 10 套风格预设

定义在 `references/style-presets.md`，沿两个轴展开：

- **Register（语域）** —— 多正式、多密
- **Domain metaphor（领域隐喻）** —— 借用哪个行业的规则

| # | 预设 | 语域 | 隐喻 |
|---|---|---|---|
| P1 | `On Roster` 在册名册 | 档案 | 登记表 / 勘验单 |
| P2 | `Blueprint` 工程图纸 | 工业 | 工程制图 |
| P3 | `Marquee` 剧场场刊 | 奢华克制 | 剧场节目单 |
| P4 | `Decision Desk` 决策编辑台 | 编辑部 | 出版编辑部 |
| P5 | `Control Plane` 运营控制平面 | 工业 | 工业控制系统 |
| P6 | `Shared Atlas` 共享数据地图 | 编辑-技术 | 地图学 |
| P7 | `Lab Bench` 实验台 | 编辑-技术 | 实验室记录 |
| P8 | `Contract` 合同/勘验单 | 粗野主义 | 法律文书 |
| P9 | `Atelier` 工坊 | 温暖人文 | 手工作坊 |
| P10 | `Terminal Ledger` 终端账本 | 工业 | 会计账簿 |

每套预设都规定了**构图、字体、材质、色彩、动效、禁止项**，以及**它最大的风险和一种低成本验证方式**。另有 6 组命名组合应对混合需求。

### 用法示例

```text
Use $ultra-ui-skill with the Blueprint preset for this product.
```

中文也可以：

```text
用 $ultra-ui-skill 的 Blueprint 工程图纸风格做这个产品界面。
```

---

## 10 套预设的实际效果

下面每张图都是**同一套固定骨架**套用不同预设的结果。骨架完全相同，是为了让预设之间能横向对比；**骨架之外的一切都是该预设自己的材质与深度语言** —— 圆角、阴影、透明度、纹理、密度、分隔方式、墨色与留白的比例。

**固定骨架**：字标 + 定位句 · 色板 · 字阶样本 · 抽象品牌几何 · 低保真产品线框 · 材质样本 · 圆角/边缘研究 · 组件样本 · 一句禁忌。

---

### P1 · On Roster 在册名册

![On Roster 预设板](assets/showcase/presets/01-on-roster.png)

*登记表语言。* 表格纪律、编号行、未涂布纸上的印章红强调。几乎没有动效；页面上一切都是可登记的事实。

---

### P2 · Blueprint 工程图纸

![Blueprint 预设板](assets/showcase/presets/02-blueprint.png)

*制图语言。* 工程网格、图纸外框、定位角标、尺寸线、图纸标题栏。精确本身就是美学。

---

### P3 · Marquee 剧场场刊

![Marquee 预设板](assets/showcase/presets/03-marquee.png)

*剧场节目单语言。* 深底 + 舞台光衰减、聚光洗、长投影；靠字号的戏剧性跨度建立层级。

---

### P4 · Decision Desk 决策编辑台

![Decision Desk 预设板](assets/showcase/presets/04-decision-desk.png)

*编辑部工作台语言。* 暖纸面、发丝分割线、页边批注。层级来自阅读顺序，而不是容器的数量。

---

### P5 · Control Plane 运营控制平面

![Control Plane 预设板](assets/showcase/presets/05-control-plane.png)

*工业控制台语言。* 哑光搪瓷细颗粒、机加工边缘、蚀刻标记。当密度对应真实机器时，密集就是合理的。

---

### P6 · Shared Atlas 共享数据地图

![Shared Atlas 预设板](assets/showcase/presets/06-shared-atlas.png)

*地图学语言。* 真·半透明层叠平面、等高线环、柔和的高程晕渲。关系本身就是主要内容。

---

### P7 · Lab Bench 实验台

![Lab Bench 预设板](assets/showcase/presets/07-lab-bench.png)

*实验室记录语言。* 方格纸作为基底、标尺图表框、精确刻度。每个数值都显示它的测量方式。

---

### P8 · Contract 合同/勘验单

![Contract 预设板](assets/showcase/presets/08-contract.png)

*记录文书语言。* 纸张牙口、硬边、零圆角、一枚物理印章压痕。任何东西都不漂浮在文档之外。

---

### P9 · Atelier 工坊

![Atelier 预设板](assets/showcase/presets/09-atelier.png)

*温暖人文的手作语言。* 亚麻纹理、漫射柔光、大圆角面板。温度来自比例与材质，而不是粉彩雾感。

---

### P10 · Terminal Ledger 终端账本

![Terminal Ledger 预设板](assets/showcase/presets/10-terminal-ledger.png)

*流水账语言。* 热敏纸点阵纹理、账本横线、等宽表格数字，绿/红配色**只**用于正负号含义。

---

> 以上均为**生成的概念图**，用于展示各预设的方向。它们不是生产环境截图，也不构成对输出质量的保证。

---

## Mosaic 视觉案例（完整设计链路）

Mosaic 是一个虚构产品，展示从设计方向 → 产品实证 → 连续交互状态的完整流程。

![Mosaic 艺术方向板：定义编辑部证据台的视觉系统](assets/showcase/01-direction-board.png)

*方向定义：视觉论点、配色、字体、布局语法与明确的禁止项，建立共识简报。*

![Mosaic 落地页：展示 Sources、Reconcile、Shared View 的产品旅程](assets/showcase/02-landing-page.png)

*落地页实证：用具象的续约风险场景演示产品旅程，而不是靠装饰性 UI。*

![Mosaic 交互序列：源检查、冲突解决、发布](assets/showcase/03-interaction-sequence.png)

*连续交互状态：同一个产品界面从源检查推进到冲突解决，再到已发布决策视图。*

> Mosaic 是虚构产品。以上是生成的概念图，用于说明 Ultra UI Skill 的工作流，不是生产截图，也不构成输出质量保证。

---

## 仓库结构

```text
ultra-ui-skill/
├── SKILL.md                  技能入口与工作流路由
├── README.md                 英文说明
├── README.zh-CN.md           中文说明（本文件）
├── agents/openai.yaml        Codex UI 元数据
├── assets/showcase/          Mosaic 概念图
│   └── presets/              10 张预设风格板
├── references/               风格预设、创意方向、评审清单、反 AI 味指南
├── evals/                    基线、启用技能后的对比结果、视觉测试夹具
└── LICENSE
```

---

## 安装

### 给 Codex

PowerShell：

```powershell
$skillsRoot = if ($env:CODEX_HOME) { Join-Path $env:CODEX_HOME "skills" } else { Join-Path $HOME ".codex\skills" }
New-Item -ItemType Directory -Force -Path $skillsRoot | Out-Null
git clone https://github.com/leoliao19911017-stack/ultra-ui-skill.git (Join-Path $skillsRoot "ultra-ui-skill")
```

POSIX shell：

```sh
skills_root="${CODEX_HOME:-$HOME/.codex}/skills"
mkdir -p "$skills_root"
git clone https://github.com/leoliao19911017-stack/ultra-ui-skill.git "$skills_root/ultra-ui-skill"
```

两种方式在未设置 `CODEX_HOME` 时都装到 `~/.codex/skills/ultra-ui-skill`。若技能未被立即识别，重启 Codex 或开新会话。

### 给 Claude Code

```sh
git clone https://github.com/leoliao19911017-stack/ultra-ui-skill.git ~/.claude/skills/ultra-ui-skill
```

---

## 使用

在提示词里显式调用：

```text
用 $ultra-ui-skill 把这个产品需求转成三个真正不同的 UI 方向，
推荐其中一个，并定义出可观察的设计简报。
```

当界面有「通用、模板化、过度装饰、一看就是 AI 生成」的风险时，它也可能被自动选用。

---

## 本地校验

```powershell
$codexHome = if ($env:CODEX_HOME) { $env:CODEX_HOME } else { Join-Path $HOME '.codex' }
$validator = Join-Path $codexHome 'skills\.system\skill-creator\scripts\quick_validate.py'
$skill = Join-Path $codexHome 'skills\ultra-ui-skill'
python $validator $skill
```

校验器来自 Codex 本地安装的 `skill-creator` 系统技能。它只检查技能打包与 frontmatter，**不证明设计质量**。

---

## 证据与边界

仓库包含[无技能基线](evals/baseline.md)与[启用技能后的评测](evals/with-skill.md)。已记录的评测覆盖了：发散式方向探索、先删减后装饰、有边界的截图评审。

这些是**少量单次运行的行为观察**，不构成可重复的视觉质量、生产就绪性，或跨模型/跨项目优越性的证明。

---

## 来源与独立性

本技能是对公开可读方法「[How to turn your AI into a world-class designer](https://www.lennysnewsletter.com/p/how-to-turn-your-ai-into-a-world)」的**独立提炼**，并补充了明确标注为「生产启发」的内容。它不复制原文。

该公开文章在 Technique 7 标题之后即被付费墙挡住。本技能**不把未读到的付费内容当作来自原文**。

风格预设是**为本技能撰写的生产启发**，建立在源文章方法之上 —— 它们**不是**原文的措辞或主张。

Ultra UI Skill 与 Lenny's Newsletter、Anshu Chimala 无隶属、赞助或背书关系。

---

## 许可证

[MIT](LICENSE)
