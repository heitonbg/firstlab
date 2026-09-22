# Словарь токенов проекта — Talking Travel

## Ширины
- Контейнер: 1200px
- Внешние поля: 24px (360), 40px (768), авто (1280)
- Контрольные ширины: 360 / 768 / 1280

## Типографика
- Основной шрифт: "Inter", system-ui, sans-serif
- Логотип «Talking»: рукописный (Sacramento / cursive), 20px
- Логотип «Travel»: гротеск, 24px, 800
- H1 (hero, статья): clamp(2rem, 1.2rem + 3vw, 3.5rem), 700
- H2 (секции): clamp(1.5rem, 1rem + 2vw, 2.25rem), 700
- H3 (карточки): 1.25rem, 600
- Body: 1rem / 1.5
- Muted: 0.875rem
- Надзаголовок (eyebrow): 0.75rem, uppercase, letter-spacing 0.08em, акцент
- Blockquote: italic, 1.125rem

## Палитра
- Текст: #1b1b1f
- Muted: #5b5b66
- Акцент: #7B5BF5
- Акцент hover: #6344E0
- Фон страницы: #ffffff
- Поверхность карточек: #f6f7f9
- Границы: #e5e7eb
- Overlay на hero-фото: rgba(0,0,0,0.35)

## Шаг отступов
0.5rem / 1rem / 2rem / 4rem (space-2, space-4, space-8, space-16)

## Радиусы и тени
- Радиус: 12px (карточки, кнопки), 8px (поля ввода), 999px (пилюли)
- Тень: 0 1px 2px rgba(0,0,0,.04), 0 8px 24px rgba(0,0,0,.06)

## Формы
- Поле ввода: фон #ffffff, граница 1px solid #e5e7eb, радиус 8px, padding 0.5rem 1rem
- Поле в фокусе: граница акцентного цвета #7B5BF5
- Кнопка submit: primary (фиолетовая)
- Форма центрирована, max-width 480px

## Blockquote
- Фон: #f6f7f9
- Левая граница: 4px solid #7B5BF5
- Padding: 1rem 1.5rem
- Радиус: 12px

## Карточки статей (Recent story)
- Большая: изображение 16:9, h3 1.5rem
- Маленькие: изображение 4:3, h3 1.125rem
- Общее: радиус 12px, тень

## Секции
- Hero: фон-фото + overlay rgba(0,0,0,0.35)
- Featured swiss: 2 колонки (фото | текст) с 768px
- Destinations: 4 колонки (1280), 2 (768), 1 (360)
- Join-form: центрированная узкая колонка max-width 480px
- Recent story: grid 2fr 1fr с 768px
- Article (blog.html): текст max-width 720px

## Повторяемые компоненты
- Кнопка (primary — фиолетовая, ghost — с play)
- Иконка play
- Поле ввода
- Форма join-form
- Карточка направления (4 варианта)
- Карточка статьи (большая / маленькая)
- Featured-блок
- Article с header/body/blockquote
- Пункт навигации
- Логотип двумя строками
- .section-title, .eyebrow

## Состояния
- hover, focus-visible, active, disabled
- Фокус: outline 2px акцентного цвета, offset 2px

## Принятые решения (чего нет в макете)
- Мобильная навигация: вертикальный список до 768px
- Логотип «Talking» рукописным шрифтом — Google Font Sacramento
- Промежуточные ширины: одноколоночная база
- Длинные заголовки: text-wrap: balance
- Hero-фон: изображение через CSS background с overlay