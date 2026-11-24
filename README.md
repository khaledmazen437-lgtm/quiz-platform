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

=================== ./README-mhd-store.md ===================
# MHD Store (private)

> متجر MHD الإلكتروني — PHP/MySQL بلوحة أدمن مبنية يدويًا (نظام ModelAdmin شبه Django admin).

A private PHP/MySQL e-commerce store with a hand-rolled admin framework: declarative `ModelAdmin` classes (list display, fieldsets) manage products, categories and store content, with image uploads and security headers + CSRF tokens on the front controller.

## Features

- Product catalog with categories, prices and discounts
- Custom admin panel (`admin.php` + `admin_config.php`) with upload handling
- PDO with prepared statements, CSRF token, and hardened HTTP headers in `index.php`

## Tech Stack

- PHP 8+ (no framework), MySQL (PDO), sessions

## Notes

- ⚠️ Database credentials are committed in `db_connect.php` — move them to environment variables and rotate the password (it was reused elsewhere and exposed).
- Restrict `uploads/` permissions (currently created with 0777).

