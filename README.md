# 🐕 Xiaonuo's Dog Learning House (小诺狗狗学习屋)

A single-page, self-contained HTML web app that turns daily homework and study habits into a gentle pet-raising game for an elementary school student.

**Live demo:** https://yun-cheng-api.github.io/xiaonuo-dog-house/

## What it does

- **Task list & rewards** – Pick a subject/task from a dropdown (math, Chinese, English, reading, etc.), set a focus timer (stopwatch-style, 15/20 min options), and complete it to earn "bones" 🦴 that feed a virtual Shiba Inu puppy.
- **Pet growth system** – The puppy grows through life stages as the daily point goal is reached; finishing tasks with ≥90% accuracy earns bonus points (double feeding).
- **Learning rainbow** – A daily progress bar across Math / Chinese / English that fills in as graded accuracy comes in, visualized as a rainbow.
- **Mini study games ("屋里练")**, each randomly drawing from a question bank:
  - 📜 **Poetry fill-in-the-blank** – Classic Tang poems (五/七言绝句 from 唐诗三百首), with pinyin and a modern Chinese explanation of the line shown only after answering.
  - 📖 **Chinese knowledge points** – Quiz bank covering Grade 3 textbook concepts.
  - 🔤 **English word matching** – Vocabulary quiz with text-to-speech pronunciation (British male voice).
  - ✏️ **Sentence ordering** – Drag-and-drop English sentence reconstruction.
  - 🧮 **Math drills** – Quick arithmetic practice.
  - ✈️ **Aviation knowledge quiz** – Fun facts about aircraft, tied to the "captain" theme.
  - 🔁 **Mistake reinforcement** – Revisits previously wrong answers, accumulated over time (not limited to the current day).
- **💭 Reflection prompts** – After finishing any mini-game, a guided two-step "think about it" pops up: a simple, concrete first question (easy to answer in a sentence) followed by a "why/how does this connect" follow-up. The goal isn't quiz accuracy — it's building the habit of summarizing, connecting old and new knowledge, and asking "why," in small steps a child can actually express.
- **🎤 Voice input** – Both the book report and the reflection answers can be filled in by speaking instead of typing (uses the browser's speech recognition; the mic button is hidden automatically on browsers that don't support it).
- **📝 Reflection journal** – Every reflection the child writes (or speaks) is saved and viewable from the 📝 button in the top bar, so progress in thinking (not just scores) is visible over time.
- **⚙️ Custom question banks** – Each family can replace any of the built-in question banks with their own content (their child's textbook, word list, books, etc.) by pasting/uploading a JSON file via the ⚙️ button. See [`QUESTION_BANK_TEMPLATE.md`](QUESTION_BANK_TEMPLATE.md) for the format — it also explains how to ask an AI assistant to generate a custom bank, and how to write good reflection prompts. Any category left out of the custom JSON falls back to the default bank.

## Tech notes

- Single `index.html` file — no build step, no backend.
- All progress, custom question banks, and reflection journal entries are stored locally in the browser (`localStorage`), so each device/browser keeps its own data.
- Hosted via GitHub Pages for easy access from any device's browser (e.g. add to home screen on iPhone Safari for an app-like experience).

## Updating

Replace `index.html` with the latest exported version and commit to the `main` branch — GitHub Pages will rebuild automatically within a minute or two.
