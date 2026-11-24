# aimingmed-poster-skill

艾名医学（AIMINGMED）品牌海报 AI 设计工作流 skill——装进任意支持 SKILL.md 规范的 AI（Claude Code、Codex、Devin、OpenCode 等），AI 即可端到端把碎片化、互相矛盾的海报需求加工成可直接出图的高质量 Prompt，并在有出图工具时直接生成验收。

## 它做什么

- **需求清洗**：剥离"做不做图""要不要字"这类矛盾指令，挖出藏在聊天记录末尾的核心禁忌
- **需求核对清单**：按 7 个维度列清单给你逐项确认——整个流程最有价值的产物
- **一次性 grill**：所有冲突一次问完，每题给 A/B/C 选项，你只回字母
- **定稿 Prompt**：连贯文段、分区叙述，可直接提交绘图工具
- **出图与验收**：环境内有支持垫图的出图工具时直接生成并按清单自验；没有则交付定稿 Prompt + 交接说明

内置两张参考图：5·20 临床试验日海报（排版/风格/Logo 参考）+ 艾名熊猫医生 IP 四视图（形象锚点）。

## 安装

把 `aimingmed-poster/` 文件夹整个复制到你 AI 的 skills 目录即可：

| AI | skills 目录 |
| --- | --- |
| Claude Code / Devin 等 | `~/.claude/skills/` 或 `~/.agents/skills/` |
| Codex | `~/.codex/skills/` |
| 其他 | 放入对应 skills 目录（任何兼容 [agentskills.io](https://agentskills.io/specification) 规范的环境） |

## 使用

正常向 AI 描述海报需求即可——越原始越好，同事发的聊天记录直接粘贴也行。AI 会自动清洗需求、列清单、问你一轮选项，最后给出定稿 Prompt 或直接出图。

## 文件结构

```
aimingmed-poster/
├── SKILL.md                          # 工作流主文件（含品牌资产、清单、模板、真实案例）
├── ref1-layout-style-520-poster.jpg  # 排版/风格/Logo/字体参考（图1）
└── ref2-panda-ip-four-views.png      # 熊猫医生 IP 四视图（图2）
```

## 注意

`ref1`、`ref2` 为艾名医学品牌资产，仅限用于生成 AIMINGMED 品牌海报。
