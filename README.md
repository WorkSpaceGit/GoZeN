# Ґо

Браузерна гра Ґо для двох гравців на одному телефоні (iPhone Safari). Все в одному файлі — без встановлення, без інтернету після першого відкриття.

## Що вміє гра

- Дошки 9×9, 13×13, 19×19
- Комі (компенсація очок) з кроком 0,5
- Підрахунок території за японськими правилами — позначення мертвих каменів, ручне маркування спірних зон
- Таймери: Фішер (час + надбавка за хід) і Бьо-йомі (основний час + кілька запасних періодів)
- Історія ходів, дзен-режим на весь екран
- Додається на головний екран iPhone як окремий застосунок

## Кольорове рішення

Все базується на темному тлі з одним фірмовим акцентом — теплим золотисто-амбровим кольором. Це не випадковий вибір: золото/амбер традиційно асоціюється з деревом і камінням для Ґо, а темне тло — стандарт для будь-якого екранного інтерфейсу.

| Елемент | Колір | Що означає |
|---|---|---|
| Фон застосунку (вкладки, панелі) | `#1f1f1e` темно-графітовий | Нейтральне тло, на якому нічого не "сліпить" |
| Дошка (ігрове поле) | `#d4a84b` теплий золотистий | Імітація дерев'яної дошки |
| Лінії сітки на дошці, координати | `#4a3206` темно-коричневий | Контраст до дерева, як на справжній дошці |
| Активна кнопка / вибраний режим (наприклад 9×9, 2+7, ⊘) | `#dcb35c` золото-амбер з рамкою | Один і той самий колір скрізь — означає "це обрано / це активне" |
| Неактивний текст (підписи "Разом", "Територія", заголовки) | `#666` / `#6a6a68` сірий | Не привертає уваги, лише довідкова інформація |
| Числа в таблиці рахунку | `#b0b0ac` світло-сірий | Трохи світліше за підписи — це вже дані, а не підпис |
| Рядок "Разом" (підсумок) | `#f0f0ec` майже білий, переможець — золотий | Найважливіший рядок таблиці виділяється і кольором, і вагою шрифту |
| Смужка історії ходів | `#c49a3a` золотистий фон | Той самий теплий тон що й дошка — це продовження партії, а не окремий блок |
| Прогрес-бар таймера (звичний стан) | `#3a2c0a` тьмяний амбер | Видно, скільки часу лишилось, але не привертає зайвої уваги |
| Прогрес-бар таймера (активний хід) | `#dcb35c` яскравий амбер | Той самий акцентний колір — зараз твоя черга |
| Критичний стан — лишилось менше 30 секунд (10 у бьо-йомі) | `#c94444` червоний | Єдиний "тривожний" колір у всьому інтерфейсі — з'являється тільки тут |

**Принцип простий:** один акцентний колір (золото) для всього, що активне чи обране, один нейтральний сірий для всього довідкового, і червоний — виключно для попередження про час. Жодних додаткових кольорів, які могли б заплутати.

---

# Go — a phone game

A browser-based two-player Go game for one phone (iPhone Safari). Everything lives in a single file — no installation, no internet needed after the first load.

## What it does

- 9×9, 13×13, and 19×19 boards
- Komi (point compensation) adjustable in steps of 0.5
- Japanese-rules territory scoring — mark dead stones, manually mark disputed areas
- Timers: Fischer (base time + bonus per move) and Byo-yomi (main time + a few backup periods)
- Move history, full-screen zen mode
- Can be added to the iPhone home screen as its own app

## Color scheme

Everything is built on a dark background with one signature accent — a warm gold/amber. This isn't arbitrary: gold and amber are traditionally tied to the wood and stones used in Go, while a dark background is the standard choice for any screen-based interface.

| Element | Color | Meaning |
|---|---|---|
| App background (panels, tabs) | `#1f1f1e` dark graphite | Neutral backdrop that doesn't compete for attention |
| Board (playing surface) | `#d4a84b` warm gold | Mimics a wooden board |
| Grid lines, coordinates on the board | `#4a3206` dark brown | Contrasts with the wood, like a real board |
| Active button / selected mode (e.g. 9×9, 2+7, ⊘) | `#dcb35c` gold-amber with outline | The same color everywhere means "this is selected / active" |
| Inactive labels ("Total", "Territory", headers) | `#666` / `#6a6a68` gray | Doesn't draw the eye — it's just reference text |
| Numbers in the score table | `#b0b0ac` light gray | Slightly brighter than labels — this is data, not a caption |
| "Total" row (final result) | `#f0f0ec` near-white, winner in gold | The most important row in the table stands out by both color and weight |
| Move history strip | `#c49a3a` golden background | Same warm tone as the board — it's a continuation of the game, not a separate block |
| Timer progress bar (normal) | `#3a2c0a` dim amber | Shows how much time is left without demanding attention |
| Timer progress bar (active turn) | `#dcb35c` bright amber | Same accent color — it's your move right now |
| Critical state — under 30 seconds left (10 in byo-yomi) | `#c94444` red | The only "alarm" color in the whole interface — appears only here |

**The principle is simple:** one accent color (gold) for anything active or selected, one neutral gray for anything informational, and red reserved strictly for time warnings. No extra colors to cause confusion.
