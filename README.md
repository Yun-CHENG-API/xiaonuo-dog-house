# 🐕 Xiaonuo's Dog Learning House (小诺狗狗学习屋)

A single-page, self-contained HTML web app that turns daily homework and study habits into a gentle pet-raising game for an elementary school student.

**Live demo:** https://yun-cheng-api.github.io/xiaonuo-dog-house/

## What it does

- **Task list & rewards** – Pick a subject/task from a dropdown (math, Chinese, English, reading, etc.), set a focus timer (stopwatch-style, 15/20 min options), and complete it to earn "bones" 🦴 that feed a virtual Shiba Inu puppy.
- **Pet growth system** – The puppy grows through life stages as the daily point goal is reached; finishing tasks with ≥90% accuracy earns bonus points (double feeding).
- **Learning rainbow** – A daily progress bar across Math / Chinese / English that fills in as graded accuracy comes in, visualized as a rainbow.
- **Mini study games ("屋里练")**, each randomly drawing from a question bank:
  - 📜 **Poetry fill-in-the-blank** – Classic Tang poems (五/七言绝句 from 唐诗三百首), with pinyin shown only after answering.
  - 📖 **Chinese knowledge points** – Quiz bank covering Grade 3 textbook concepts.
  - 🔤 **English word matching** – Vocabulary quiz with text-to-speech pronunciation (British male voice).
  - ✏️ **Sentence ordering** – Drag-and-drop English sentence reconstruction.
  - 🧮 **Math drills** – Quick arithmetic practice.
  - ✈️ **Aviation knowledge quiz** – Fun facts about aircraft, tied to the "captain" theme.
  - 🔁 **Mistake reinforcement** – Revisits previously wrong answers, accumulated over time (not limited to the current day).

## Tech notes

- Single `index.html` file — no build step, no backend.
- All progress is stored locally in the browser (`localStorage`), so each device/browser keeps its own progress.
- Hosted via GitHub Pages for easy access from any device's browser (e.g. add to home screen on iPhone Safari for an app-like experience).

## Updating

Replace `index.html` with the latest exported version and commit to the `main` branch — GitHub Pages will rebuild automatically within a minute or two.
