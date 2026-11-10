# 📚 exam-quiz-app

<a id="chinese"></a>

**简体中文** | [English](#english)

> 期末周人类续命工具 —— 一个让 Claude 帮你把复习资料变成刷题软件的 Skill。

老师发来 80 页 PPT，说“重点都在里面了”。
你打开一看，确实都在里面了 —— **问题是全都在里面了。**

这个 Skill 就是为这种时刻准备的：把 PPT、PDF、Word、考试大纲丢给 Claude，几分钟后你会得到一个**能离线运行的刷题软件**（单个 HTML 文件，双击就能打开，断网也不怕）。

---

## ✨ 它能干什么

| 功能 | 说明 |
| --- | --- |
| 📝 严格按原题 | 题型、题号、原文、答案一个字不改，不偷偷加题。老师出什么，你就刷什么 |
| 💡 每题都有解析 | 选择题告诉你为什么选、别的选项错在哪；计算题从“这是个啥”讲起 |
| 🧮 零基础详解 | 专为“上课在听，但没听懂”的同学设计：概念白话 → 分步算式 → 必背公式 |
| 🎯 简答题采分点 | 长篇答案压缩成加粗关键词，背得下来才是好答案 |
| 🃏 练题 / 背题模式 | 像背单词一样一屏一题：错题隔 3 题再考你，答对后隔 8 题再确认一次，一次就对的直接毕业。背题模式先看答案再默写 |
| ❌ 错题本 | 做错自动收录，做对自动移出，比你记得清楚 |
| 🔍 搜题 | `Ctrl/⌘ + K` 搜关键词，考前十分钟找题神器 |
| 📊 章节掌握度 | 每章刷了多少一目了然，自我欺骗难度 +100% |
| 🔮 考试预测 | 根据你的练习记录估算能考几分、能不能过，还告诉你哪类题提分最快。准不准另说，扎心是真的 |
| 🎨 外观切换 | 白天、黑夜、护眼米黄、樱花粉、黑黄撞色……总有一款让你愿意多刷两题 |
| 🧪 模拟考试 | 原题随机组卷、计时、交卷自动判分，提前体验分数带来的冲击 |
| 🎲 额外练习 | 按原题型随机出数字的同类题，并且老实标明“不是原题” |
| 📱 手机 / 深色模式 | 床上刷、地铁刷、凌晨三点关灯刷 |

---

## ⌨️ 全键盘操作（鼠标可以退休了）

| 按键 | 作用 |
| --- | --- |
| `Ctrl/⌘ + Enter` | 显示答案，再按一次下一题 |
| `1` – `5` | 选择题直接选 |
| `Enter` / `→` | 下一题 / 跳到下一个空 / 提交多选 |
| `Ctrl/⌘ + K` | 打开搜题 |
| `Shift + Enter` | 简答题换行 |

看完答案后光标会自动回到第一个空 —— 从头到尾不用碰鼠标，效率高到有点不像在学习。

---

## 🚀 安装

**claude.ai / Claude 桌面版**

1. 下载本仓库里的 `exam-quiz-app.zip`
2. 打开 设置 → Capabilities → Skills，上传它

**Claude Code**

```bash
cp -r exam-quiz-app ~/.claude/skills/
```

---

## 🗣️ 使用

把复习资料发给 Claude，然后说：

```text
帮我生成刷题软件
```

或者更真实一点：

```text
我明天早上考试，现在什么都不会，救一下
```

两种说法都能用。第二种 Claude 还会顺便给你排一个复习顺序。

---

## 🧠 设计原则

1. **原题至上**：资料里的答案就算有错，也只在解析里加“注：……”，不擅自改。考试按老师的答案判分，不按 AI 的。
2. **诚实标注**：资料里没给答案的题，会明确告诉你哪些答案是 Claude 写的，方便你找老师核对。
3. **先能用，再好看**：单个 HTML 文件，不装任何东西，U 盘拷走就能用。

---

## 📁 文件结构

```text
exam-quiz-app/
├── exam-quiz-app/
│   └── SKILL.md          # 技能本体：流程、出题原则、功能清单
├── exam-quiz-app.zip     # 打包好的 Skill，可直接上传
└── README.md             # 你正在看的这个（中文在前，英文在后）
```

---

## ⚠️ 免责声明

- 本工具能提高你的复习效率，但**不能替你去考试**。
- 刷题本里的“已掌握”只代表你点了“会了”，不代表你真的会了。
- 如果考前一晚才发现这个仓库，那也比没发现强。

---

## 🙋 作者

**Derrick** —— 在考前 72 小时内被 5 门课追着跑，于是做了这个东西。

如果它帮你多拿了几分，欢迎点个 ⭐。
如果没帮上……那一定是复习时间不够 🙃

---

<a id="english"></a>

# 📚 exam-quiz-app (English)

[简体中文](#chinese) | **English**

> A life-support system for finals week — a Claude Skill that turns your revision materials into a quiz app.

Your professor sends over an 80-slide deck and says, "Everything you need is in there."
You open it. Everything *is* in there. **That's exactly the problem.**

This Skill is built for that moment. Hand Claude your slides, PDFs, Word docs or syllabus, and a few minutes later you get an **offline quiz app** — a single HTML file you can double-click to open, no internet required.

---

## ✨ What it does

| Feature | Description |
| --- | --- |
| 📝 Faithful to the source | Question types, numbering, wording and answers stay exactly as given. No sneaky extra questions — you drill what your professor wrote |
| 💡 Explanations for every question | Multiple choice explains why the answer is right *and* why the others are wrong; calculations start from "what even is this" |
| 🧮 Zero-background walkthroughs | For students who attended every lecture and understood none of them: plain-language concept → step-by-step working → formulas to memorize |
| 🎯 Short-answer scoring points | Long model answers condensed into bold keywords. An answer you can't memorize isn't a good answer |
| 🃏 Drill & Learn modes | Flashcard-style, one question per screen: a miss comes back 3 questions later, a fixed miss returns once more 8 questions later, and first-try hits graduate immediately. Learn mode shows the answer first, then makes you recall it |
| ❌ Mistake notebook | Wrong answers are saved automatically and removed once you get them right. It remembers better than you do |
| 🔍 Search | `Ctrl/⌘ + K` to search questions, options and answers — perfect for the last ten minutes before the exam |
| 📊 Chapter mastery | See how far along you are in each chapter. Self-deception difficulty: +100% |
| 🔮 Pass predictor | Estimates your score and whether you will pass based on your practice record, and points to the fastest way to gain points. Accuracy debatable; emotional damage guaranteed |
| 🎨 Themes | Light, dark, sepia, sakura pink, black-and-yellow… one of them will make you want to do two more questions |
| 🧪 Mock exam | Random papers built from the original questions, timed and auto-graded. Experience the score shock early |
| 🎲 Extra practice | Same question types with randomized numbers, clearly labeled "not an original question" |
| 📱 Mobile & dark mode | Study in bed, on the subway, or at 3 a.m. with the lights off |

---

## ⌨️ Keyboard-only workflow (your mouse can retire)

| Key | Action |
| --- | --- |
| `Ctrl/⌘ + Enter` | Reveal the answer; press again for the next question |
| `1` – `5` | Pick an option |
| `Enter` / `→` | Next question / next blank / submit a multi-select |
| `Ctrl/⌘ + K` | Open search |
| `Shift + Enter` | New line in short-answer mode |

After the answer is revealed, the cursor jumps back to the first blank, so you never touch the mouse. It's so efficient it barely feels like studying.

---

## 🚀 Installation

**claude.ai / Claude desktop app**

1. Download `exam-quiz-app.zip` from this repository
2. Go to Settings → Capabilities → Skills and upload it

**Claude Code**

```bash
cp -r exam-quiz-app ~/.claude/skills/
```

---

## 🗣️ Usage

Send Claude your revision materials and say:

```text
Make me a quiz app from these
```

Or, more realistically:

```text
My exam is tomorrow morning and I know nothing. Help.
```

Both work. With the second one, Claude will also put together a study plan for the time you have left.

> The Skill's instructions are written in Chinese, but Claude understands them fine — you can talk to it in English and get an English quiz app.

---

## 🧠 Design principles

1. **The source is sacred.** Even if the materials contain a mistake, the answer isn't changed — Claude only adds a "Note: …" in the explanation. Your exam is graded by your professor's answer key, not by an AI.
2. **Honest labeling.** When the materials don't include answers, Claude tells you exactly which answers it wrote, so you can check them with your professor.
3. **Useful first, pretty second.** One HTML file, nothing to install. Copy it to a USB stick and you're good to go.

---

## 📁 Repository layout

```text
exam-quiz-app/
├── exam-quiz-app/
│   └── SKILL.md          # The skill itself: workflow, question rules, feature list
├── exam-quiz-app.zip     # Packaged skill, ready to upload
└── README.md             # You are here (Chinese first, English below)
```

---

## ⚠️ Disclaimer

- This tool makes your revision more efficient. It **cannot take the exam for you**.
- "Mastered" in the app only means you clicked "got it". It does not mean you actually got it.
- Finding this repo the night before your exam is still better than not finding it at all.

---

## 🙋 Author

**Derrick** — chased by five courses in the 72 hours before finals, and built this along the way.

If it earned you a few extra points, a ⭐ would be appreciated.
If it didn't… you probably just needed more time to revise 🙃
