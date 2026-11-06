# portfolio

Сайт-портфолио: https://logreus-cloud.github.io/portfolio/

Одна страница `index.html` без сборки и зависимостей. Шрифт JetBrains Mono подтягивается
из Google Fonts, стили внутри файла, баннер и карточка-правило лежат SVG в `assets/`.

Дизайн повторяет язык профиля [github.com/logreus-cloud](https://github.com/logreus-cloud):
палитра Primer (`#0d1117`, рамки `#30363d`, синий `#4493f8`), моноширинный баннер,
двухколоночный профильный layout и карточки репозиториев. Светлая тема включается по
`prefers-color-scheme`, на ширине до 600px подставляется высокая карточка-правило.

## Посмотреть локально

Открыть `index.html` двойным кликом, либо поднять сервер:

    python -m http.server 8765

и зайти на http://localhost:8765/

## Публикация

Репозиторий развёрнут на GitHub Pages из ветки `main`, папка `/ (root)`.
Обновление сайта: обычный пуш в `main`, Pages пересобирает страницу за минуту-две.

## Что править

- Имя и подпись: `<aside class="side">`. Баннер: блок `.banner` и `assets/banner*.svg`.
- Проекты: карточки `<article class="repo">`. Бейдж `Public` / `Private` меняется текстом.
- Стек: блок `.tech`.
- Цвета: переменные в `:root` вверху `<style>`, светлая тема в `@media (prefers-color-scheme: light)`.

Содержимое сайта повторяет README профиля (репозиторий `logreus-cloud/logreus-cloud`), поэтому
проекты и стек правятся в обоих местах. Баннер и карточки взяты оттуда же.
