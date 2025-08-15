# Metamekhanika · Serpentine (no-build)

Лёгкая мини‑игра на чистом Canvas без сборщиков. Один файл `index.html`.
Подходит для GitHub Pages / Netlify / Vercel, а также для встраивания в Tilda через `<iframe>`.

## Запуск локально
Откройте `index.html` в браузере. Для корректной работы на iOS лучше открыть через локальный сервер:
```bash
python3 -m http.server 8080
# затем: http://localhost:8080/
```

## Деплой на GitHub Pages
1. Создайте репозиторий, например `serpentine`.
2. Загрузите `index.html` в корень.
3. В настройках включите Pages (Branch: `main`, Folder: `/root`).
4. Откройте выданный URL — игра готова.

## Деплой на Netlify
Перетащите папку с `index.html` в Netlify Drop (app.netlify.com/drop).

## Встраивание в Tilda
1. Залейте игру на GitHub Pages / Netlify.
2. На странице Tilda добавьте **Zero Block → HTML** и вставьте:
```html
<iframe src="https://ВАШ-ДОМЕН/"
        style="width:100%;height:80vh;border:0;border-radius:20px;overflow:hidden"
        allow="gamepad *; fullscreen *;"
        loading="lazy"></iframe>
```
Высоту/скругление подберите под макет. Игра адаптируется под мобильный экран (9:16).

## Кастомизация
Цвета и логотип: правьте блок `COLORS` и функцию `LOGO_DRAW` внизу `index.html`.
