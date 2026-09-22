# Декомпозиция макета Talking Travel

## index.html (Home Page)

| № | Секция | Тег | Содержимое | Общие с blog.html |
|---|--------|-----|------------|-------------------|
| 1 | header | <header> | Логотип "Talking / Travel", nav (Home, Story, Gallery, Contact Us), иконки поиска и профиля | да |
| 2 | hero | <section> | Фон-фото, h1 "Let's talk about your next trip!", подзаголовок, кнопка "Share your story", кнопка "Watch highlights" с play | нет |
| 3 | featured | <section> | Фото Маттерхорна, надзаголовок "FEATURED DESTINATION", h2 "Our swiss adventure blog", текст, ссылка "Watch Now" | нет |
| 4 | destinations | <section> | h2 "Discover the world with us", сетка 4 карточек: Iceland, Italy, Dubai, Patagonia | нет |
| 5 | join-form | <section> | h2 "Join our next destination", форма (имя, email, submit) | да |
| 6 | recent | <section> | h2 "Recent story writing", 1 большая + 2 маленькие карточки статей | нет |
| 7 | footer | <footer> | Nav, копирайт | да |

## blog.html (Blog article page)

| № | Секция | Тег | Содержимое | Переиспользуется |
|---|--------|-----|------------|------------------|
| 1 | header | <header> | Идентично index.html | да |
| 2 | article-header | <header> | h1 "Hello Switzerland!", обложка, автор, дата, иконка play | нет |
| 3 | article-body | <section> | h2 "My Swiss adventure story", текст | нет |
| 4 | blockquote | <blockquote> | Цитата + CTA | нет |
| 5 | adventure | <section> | h2 "Adventure", 3 фото + текст | нет |
| 6 | join-form | <section> | Та же форма, что на главной | да |
| 7 | footer | <footer> | Идентично index.html | да |

## Повторяемые компоненты
- .site-header, .site-nav, .logo, .icon-button
- .button (--primary, --ghost)
- .icon-play
- .destination-card (4 варианта)
- .story-card (большая / маленькая)
- .join-form (на обеих страницах)
- .article-header, .article-body, .blockquote
- .section-title, .eyebrow, .container

## Границы блоков
- Карточка направления = <article>.
- Статья = <article> внутри <main>.
- Форма = <form> внутри <section aria-labelledby>.
- Hero = <section> с CSS background-image.

## Спорные случаи (решения)
- Логотип: <a> с двумя <span>.
- Иконки поиска/профиля: <button aria-label>.
- Discover: <a> на якорь в blog.html.
- Watch highlights / Watch Now: <a> с иконкой play.
- Hero-фон: CSS background-image + overlay.
- blog.html — статья, а не список.