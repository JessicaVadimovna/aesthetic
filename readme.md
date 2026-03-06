# ARCHITECT // PREMIUM

Премиальный одностраничный минималистичный веб-сайт с современным дизайном в стиле брутализма и минимализма. Идеально подходит для архитектурных бюро, дизайн-студий и креативных агентств.

---

## 🎨 О проекте

**ARCHITECT // PREMIUM** — это высококачественный веб-сайт с фокусом на визуальный опыт и интерактивность. Проект демонстрирует современные подходы к веб-дизайну, сочетая строгость линий, премиальные анимации и безупречную адаптивность.

### 🌟 Ключевые особенности

- **🎯 Премиальный дизайн** — строгая геометрия, инженерная эстетика
- **🖱️ Кастомный двойной курсор** — элегантный и функциональный
- **🎬 Scroll-анимации** — плавные эффекты появления элементов
- **🌓 Темная/светлая тема** — переключение с сохранением в localStorage
- **📱 Полная адаптивность** — от 320px до 4K экранов
- **⚡ Высокая производительность** — оптимизированные анимации
- **🎥 Видео-контент** — интеграция HD видео с эффектами

---

## 🛠️ Технологии

### Frontend

- **HTML5** — семантическая разметка
- **CSS3** — современные возможности стилизации
  - CSS Grid & Flexbox
  - CSS Custom Properties (переменные)
  - CSS Transitions & Animations
  - CSS Filters & Blend Modes
- **Vanilla JavaScript** — без зависимостей
  - ES6+ синтаксис
  - Intersection Observer API
  - RequestAnimationFrame
  - LocalStorage API

### Шрифты

- **Cinzel** (Google Fonts) — заголовки и акценты
- **Space Grotesk** (Google Fonts) — основной текст

### Медиа-ресурсы

- **Unsplash** — высококачественные изображения
- **Pexels** — HD видео контент

---

## 🎭 Дизайн-система

### Цветовая палитра

#### Светлая тема

```css
--bg: #fafafa /* Основной фон */ --bg-secondary: #ffffff /* Вторичный фон */
  --fg: #0a0a0a /* Основной текст */ --fg-secondary: #666666
  /* Вторичный текст */ --line: rgba(10, 10, 10, 0.08) /* Линии и границы */;
```

#### Темная тема

```css
--bg: #0a0a0a /* Основной фон */ --bg-secondary: #141414 /* Вторичный фон */
  --fg: #f0f0f0 /* Основной текст */ --fg-secondary: #999999
  /* Вторичный текст */ --line: rgba(255, 255, 255, 0.08) /* Линии и границы */;
```

### Типографика

- **Заголовки**: Cinzel, размер от 2rem до 10rem
- **Основной текст**: Space Grotesk, размер 0.9-1.05rem
- **Межстрочный интервал**: 1.7-1.9
- **Tracking**: от -0.025em до 0.2em

### Анимации

- **Easing**: cubic-bezier(0.19, 1, 0.22, 1)
- **Duration**: 0.3s - 1.2s
- **Scroll animations**: Intersection Observer с threshold 0.15

---

## 🎬 Реализованные эффекты

### 1. Кастомный курсор

- Двойной курсор (основной + контур)
- Плавное следование за мышью с задержкой
- Эластичное увеличение при hover
- Mix-blend-mode: difference для контраста
- Темный курсор на светлой теме / светлый на темной

### 2. Scroll-анимации

- **fadeInUp** — появление снизу с движением вверх
- **scroll-reveal** — универсальное появление
- **scroll-reveal-left/right** — появление с боков
- **scroll-scale** — масштабирование с задержкой
- **Parallax** — легкий эффект глубины для медиа

### 3. Hover-эффекты

- Трансформация и масштабирование
- Анимированная заливка кнопок
- Переход цвета изображений (grayscale → color)
- Магнитная кнопка (следует за курсором)
- Hacker text effect (рандомные буквы)

### 4. UI компоненты

- Sticky header с эффектом сжатия
- Progress bar (прогресс скролла)
- Живые часы (real-time)
- Анимированный noise overlay
- Responsive grid background

---

## 📱 Адаптивность

### Breakpoints

```css
/* Десктоп */
> 1700px  /* Максимальная ширина контейнера */

/* Планшет */
≤ 768px   /* Вертикальная раскладка, упрощенная навигация */

/* Мобильный */
≤ 380px   /* Оптимизация для малых экранов (320px) */
```

### Мобильные оптимизации

- Отключение кастомного курсора
- Отключение тяжелых эффектов (noise, parallax)
- Упрощенные анимации
- Вертикальная раскладка галереи
- Адаптивные размеры шрифтов (clamp)
- Компактные отступы

---

## ⚡ Производительность

### Оптимизации

- **RequestAnimationFrame** для всех анимаций
- **Intersection Observer** вместо scroll listeners
- **will-change** для GPU-ускорения
- **backface-visibility: hidden** для 3D трансформаций
- Условное отключение эффектов на мобильных
- Lazy loading подход к анимациям

### Метрики

- **First Contentful Paint**: < 1.5s
- **Time to Interactive**: < 3s
- **Lighthouse Score**: 90+

---

## 🚀 Использование

### Быстрый старт

```bash
# Клонируйте файл
git clone architect-premium.html

# Откройте в браузере
open architect-premium.html
```

### Требования

- Современный браузер (Chrome 90+, Firefox 88+, Safari 14+)
- JavaScript включен
- Интернет-соединение (для шрифтов и медиа)

### Настройка

#### Изменить цветовую схему

```css
:root {
  --bg: #ваш-цвет;
  --fg: #ваш-цвет;
  --accent: #ваш-цвет;
}
```

#### Изменить размер курсора

```css
:root {
  --cursor-size: 32px; /* Измените значение */
}
```

#### Добавить свой контент

```html
<article class="article-block trigger scroll-reveal">
  <!-- Ваш контент -->
</article>
```

---

## 🎯 Структура проекта

```
architect-premium.html
├── <head>
│   ├── Meta tags
│   ├── Google Fonts
│   └── <style>
│       ├── Variables
│       ├── Global styles
│       ├── Components
│       ├── Animations
│       └── Media queries
│
├── <body>
│   ├── Noise overlay
│   ├── Custom cursor (dual)
│   ├── Progress bar
│   │
│   └── <div class="container">
│       ├── Header (sticky)
│       ├── Hero section
│       ├── Editorial section
│       ├── Gallery strip
│       ├── CTA section
│       └── Footer
│
└── <script>
    ├── Cursor animation
    ├── Magnetic button
    ├── Hacker text effect
    ├── Theme toggle
    ├── Scroll progress
    ├── Header scroll effect
    ├── Scroll reveal animations
    ├── Clock update
    └── Parallax effect
```

---

## 🎨 Используемые паттерны

### CSS

- **BEM-подобная** структура классов
- **Mobile-first** подход
- **CSS Custom Properties** для темизации
- **Composition over inheritance**

### JavaScript

- **Event delegation** где возможно
- **RAF (RequestAnimationFrame)** для анимаций
- **Debouncing** для scroll events
- **Observer pattern** для scroll reveals

---

## 🔧 Кастомизация

### Добавить новую секцию

```html
<section class="editorial-section">
  <aside class="sticky-col scroll-reveal-left">
    <div class="chapter-title">Chapter 02</div>
    <p class="chapter-desc">Описание главы</p>
  </aside>

  <div class="scroll-col">
    <article class="article-block trigger scroll-reveal">
      <!-- Контент -->
    </article>
  </div>
</section>
```

### Изменить scroll-анимации

```javascript
const observerOptions = {
  threshold: 0.15, // Когда начинать анимацию
  rootMargin: "0px 0px -50px 0px", // Отступы
};
```

### Добавить новый цвет в палитру

```css
:root {
  --custom-color: #ff6b6b;
}

body.dark-mode {
  --custom-color: #ff8787;
}
```

---

## 📊 Browser Support

| Browser | Version |
| ------- | ------- |
| Chrome  | 90+     |
| Firefox | 88+     |
| Safari  | 14+     |
| Edge    | 90+     |
| Opera   | 76+     |

### Не поддерживаются

- Internet Explorer (все версии)
- Старые мобильные браузеры (<2020)

---

## 🐛 Известные проблемы

### Решенные

- ✅ Двойная полоса прокрутки
- ✅ Подскакивание в конце страницы
- ✅ Плохая видимость курсора на светлой теме
- ✅ Проблемы с адаптивностью на 320px

### В работе

- ⏳ Оптимизация для очень старых устройств
- ⏳ Fallback для браузеров без Intersection Observer

---

## 🎓 Обучающие материалы

Этот проект демонстрирует:

- Modern CSS techniques (Grid, Custom Properties, Filters)
- Vanilla JavaScript animations
- Performance optimization
- Mobile-first responsive design
- Accessibility basics
- Progressive enhancement

---

## 📝 Лицензия

MIT License - используйте свободно для личных и коммерческих проектов.

---

## 👨‍💻 Автор я

Создано с ❤️ для демонстрации современных веб-технологий.

**Год**: 2026  
**Стиль**: Brutalism / Minimalism  
**Подход**: Premium / Interactive

---

## 🙏 Благодарности

- **Google Fonts** — за прекрасные шрифты
- **Unsplash** — за качественные фотографии
- **Pexels** — за HD видео контент
- **Web animations community** и **черно белым электронным книгам** — за вдохновение

---

## 📮 Контакты

Вопросы и предложения приветствуются!))

**System Status**: Operational ✓

---

_"Архитектура — это музыка застывшая в камне"_ — Иоганн Вольфганг фон Гёте

