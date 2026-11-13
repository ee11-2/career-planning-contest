# 职业规划大赛报名助手（WorkBuddy Skill）

全国大学生职业规划大赛（zgs.chsi.com.cn）全流程技能：
**读通知 → 判定赛道组别 → 生成生涯发展报告 PDF 与展示 PPT → 平台填表上传 → 生涯闯关 → 交差截图打包**。

## 安装

下载 `career-planning-contest.zip`，解压到：

```
~/.workbuddy/skills/
```

或者直接把 zip 丢给你的 AI，说一句「把这个 skill 装上，解压到 ~/.workbuddy/skills/」。

解压后目录应为 `~/.workbuddy/skills/career-planning-contest/SKILL.md`。

## 包含什么

| 目录 | 内容 |
|---|---|
| `scripts/` | 浏览器常驻驱动（driver/send/ops）、报告 PDF 生成、12 页 PPTX 生成、SVG 图表、截图打包 |
| `references/` | 平台地图（URL 与字段全表）、18 条踩坑记录、内容模板（选职业原则 / 报告三段式 / 闯关问答） |
| `assets/` | A4 报告样式、16:9 演示样式、正文骨架、给客户的交付说明模板 |

## 三件它最擅长的判断

1. **组别别选错**：专科 = 职教组，选成高教组等于白填
2. **目标职业是主轴**：先定方向再写字，否则 2000 字全废
3. **卡住了先判断是"我操作不对"还是"平台没内容"**：数一下 DOM 里的输入框数量就知道

## 边界

材料内容需真实。本技能只做**组织与排版**，不代造获奖、访谈、实习等事实。
`

## 环境

Python 3.10+，`playwright`（`playwright install chromium`）、`pypdf`、`python-pptx`、`pillow`。
导出 PDF 走 Chromium，不需要本机装 Chrome 或 LibreOffice。
