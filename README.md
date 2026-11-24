 MHD Quiz Platform

> منصة MHD للاختبارات — اختبارات اختيار من متعدد بتصحيح فوري، مبنية بصفحة واحدة وبنك أسئلة JSON.

A single-page Arabic (RTL) quiz/exam app. All questions live in `questions.json`, so adding a new subject means adding data, not code.

## Features

- Multiple-choice exams loaded from a JSON question bank (`questions.json`, ~84 KB)
- Instant scoring and answer feedback
- Clean card-based UI with the Cairo font
- No build step — open `index.html` and it runs

## Tech Stack

- Vanilla HTML/CSS/JS (all logic inline in `index.html`)
- JSON-driven content

## Running

Open `index.html` in a browser, or serve the folder with any static server:

```bash
npx serve .
```

## Notes

- Rename history: previously published as `markiting`.
- Next steps if you revisit it: timer mode, per-subject selection screen, and saving scores to localStorage.
