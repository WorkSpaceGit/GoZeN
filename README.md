# Ґо / Go

Мінімалістична гра Ґо для локального використання. Один HTML-файл — нічого зайвого.

---

## Особливості

**Дзен-режим** — серце цього проєкту. Одна кнопка прибирає весь інтерфейс і залишає лише дошку з каменями. Жодних цифр, жодного тексту, жодних кнопок — тільки гра тут і зараз. Координати на дошці також зникають. Вихід з дзену — та сама кнопка.

**Мінімалізм як принцип** — три кольори: темний фон, гобан-жовтий, чорний/білий текст. Все інше похідне. Жодних градієнтів інтерфейсу, жодних тіней на тексті, жодних зайвих елементів.

**Повна логіка гри** — японська система підрахунку, правило ко через Zobrist hashing, автоматичне визначення території, ручне коригування мертвих каменів, комі 6.5 (змінюється).

**Дошки** — 9×9, 13×13, 19×19. Вибір запускає нову гру.

**Адаптивність** — портрет: дошка зверху, панель знизу. Альбом: дошка зліва, панель справа. Орієнтовано на iPhone 16e.

**Ефективність** — камені рендеряться через offscreen-canvas і `drawImage()`, тіні рахуються один раз при зміні розміру. Інкрементальна історія ходів — DOM не перебудовується кожного ходу. Територія рахується один раз при вході в режим маркування. Canvas з `alpha:false` і `desynchronized:true`.

**PWA** — працює офлайн, додається на домашній екран, service worker кешує файл.

**Аудіо** — синтезований клік через Web Audio API, три рядки коду, нуль зовнішніх файлів.

---

## Використання

Відкрийте `go.html` у браузері. Інтернет не потрібен.

---
---

# Go

A minimalist Go game for local use. One HTML file — nothing extra.

---

## Features

**Zen mode** — the heart of this project. One button removes the entire interface, leaving only the board and stones. No numbers, no text, no buttons — just the game, here and now. Board coordinates disappear too. Exit zen with the same button.

**Minimalism as principle** — three colors: dark background, goban yellow, black/white text. Everything else derived. No interface gradients, no text shadows, no unnecessary elements.

**Full game logic** — Japanese scoring, ko rule via Zobrist hashing, automatic territory detection, manual dead stone correction, komi 6.5 (adjustable).

**Board sizes** — 9×9, 13×13, 19×19. Selecting a size starts a new game.

**Responsive** — portrait: board top, panel bottom. Landscape: board left, panel right. Optimized for iPhone 16e.

**Performance** — stones rendered via offscreen canvas and `drawImage()`, shadows computed once on resize. Incremental move history — DOM is not rebuilt on every move. Territory computed once on entering marking mode. Canvas with `alpha:false` and `desynchronized:true`.

**PWA** — works offline, installable to home screen, service worker caches the file.

**Audio** — synthesized click via Web Audio API, three lines of code, zero external files.

---

## Usage

Open `go.html` in a browser. No internet required.
