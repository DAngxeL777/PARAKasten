# PARAKasten
🚀 Obsidian Zettelkasten + PARA Template — это готовый к использованию vault, объединяющий порядок PARA (Projects, Areas, Resources, Archive) и глубину классического Zettelkasten (Fleeting → Literature → Permanent).

<div align="center">

# 🗂️ Obsidian Zettelkasten + PARA Template

**Готовая система заметок: PARA для организации + Zettelkasten для мышления.**

Шаблоны Areas, Projects, атомарных заметок и Templates.

[![Obsidian](https://img.shields.io/badge/Obsidian-1.5%2B-7C3AED?logo=obsidian&logoColor=white)](https://obsidian.md)
[![Templater](https://img.shields.io/badge/Plugin-Templater-4B8BBE)](https://github.com/SilentVoid13/Templater)
[![Dataview](https://img.shields.io/badge/Plugin-Dataview-4B8BBE)](https://github.com/blacksmithgu/obsidian-dataview)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

</div>

---

## ✨ Что это

Шаблон для Obsidian, который комбинирует две методологии:

- **PARA** — Projects, Areas, Resources, Archives — для организации всего, что требует действия.
- **Zettelkasten** — атомарные заметки со связями — для накопления и развития идей.

Вместо «свалки папок» ты получаешь систему, где **каждая заметка знает своё место**, а идеи связываются между собой через `[[wiki-links]]`.

---

## 🧭 Философия системы

| Слой | Что хранит | Формат |
|------|-----------|--------|
| **Projects** | Задачи с дедлайном и результатом | Папка + шаблон проекта |
| **Areas** | Сферы ответственности без конца (здоровье, финансы…) | MOC-заметки |
| **Resources** | Справочные материалы, темы | Тематические заметки |
| **ZK (внутри Resources)** | Конвейер мыслей | См. структуру ниже |
| **Archives** | Завершённое и неактивное | Папка |

### 🧠 Конвейер Zettelkasten (внутри `Resources/ZK`)

Твой Zettelkasten работает по классической схеме потока заметок:

1. **`00 - Meta`** — служебные заметки, правила ведения ZK, индексы.
2. **`01 - Fleeting Note`** — быстрые, мимолетные мысли (инбокс ZK). Здесь не нужно писать красиво, главное — зафиксировать.
3. **`02 - Literature Note`** — конспекты книг, статей, видео. Свои мысли по поводу источника.
4. **`03 - Permanent Note`** — **ядро системы**. Одна мысль = одна заметка. Сформулирована своими словами, имеет уникальный ID и ссылки `[[...]]` на другие постоянные заметки.
4. **`04 - Structure`** — MOC (Maps of Content) для ZK. Заметки-хабы, которые собирают Permanent Notes по темам (например, «Продуктивность», «Психология»).

> 💡 **Правило ZK:** Permanent Note не живет в папке проекта или области. Она живет в ZK и связывается ссылками. Area и Projects *ссылаются* на неё, когда нужна.

---

## 📁 Структура репозитория

```text
.
├── _Inbox/                         # Входящие заметки
├── 1. Projects/                    # Активные проекты
│   └── PROJECTS (Проекты).md       # MOC проектов
├── 2. Areas/                       # Сферы ответственности
│   ├── 00 - базовый каркас.md      # Шаблон/каркас Area
│   ├── 01 - Здоровье.md
│   ├── 02 - Финансы.md
│   ├── 03 - Быт и среда.md
│   ├── 04 - Развитие.md
│   ├── 05 - Отношения.md
│   ├── 06 - Личное управление.md
│   ├── 07 - Досуг и восстановление.md
│   └── AREAS (Сферы ответственности).md
├── 3. Resources/                   # Справочные материалы
│   ├── ZK/                         # Твой Zettelkasten
│   │   ├── 00 - Meta
│   │   ├── 01 - Fleeting Note
│   │   ├── 02 - Literature Note
│   │   ├── 03 - Permanent Note
│   │   └── 04 - Structure
│   └── RESOURCES (Ресурсы).md
├── 4. Archive/                     # Завершенные проекты
│   └── ARCHIVE (Архив).md
├── IMG/                            # Картинки и вложения
├── Templates/                      # Шаблоны Templater
│   ├── 🧚🏻‍♀️ Structure note.md
│   ├── 🪐 Permanent note.md
│   ├── ✨ Literature note.md
│   └── 🌼 Fleeting note.md
└── README.md
