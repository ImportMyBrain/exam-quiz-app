# 📚 exam-quiz-app

[简体中文](README.md) | **English**

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
| ❌ Mistake notebook | Wrong answers are saved automatically and removed once you get them right. It remembers better than you do |
| 🔍 Search | `Ctrl/⌘ + K` to search questions, options and answers — perfect for the last ten minutes before the exam |
| 📊 Chapter mastery | See how far along you are in each chapter. Self-deception difficulty: +100% |
| 🧪 Mock exam | Random papers built from the original questions, timed and auto-graded. Experience the score shock early |
| 🎲 Extra practice | Same question types with randomized numbers, clearly labeled "not an original question" |
| 📱 Mobile & dark mode | Study in bed, on the subway, or at 3 a.m. with the lights off |

---

## ⌨️ Keyboard-only workflow (your mouse can retire)

| Key | Action |
| --- | --- |
| `Ctrl/⌘ + Enter` | Reveal the answer; press again for the next question |
| `1` – `5` | Pick an option |
| `Enter` | Next question / next blank / submit a multi-select |
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
├── README.md             # Chinese README
└── README.en.md          # You are here
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
