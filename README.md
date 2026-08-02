# Анастасия — репетитор по русскому языку

Лендинг репетитора по русскому языку (подготовка к ЕГЭ, ОГЭ, итоговому сочинению, повышение успеваемости).

## Сайт

Опубликован на GitHub Pages:

- **https://sashka350.github.io/**

Репозиторий: https://github.com/Sashka350/Sashka350.github.io

## Структура проекта

```
.
├── index.html        — страница сайта
├── style.css         — стили
├── photo_*.jpg       — фотографии
└── .gitignore        — исключённые файлы (см. ниже)
```

## Как обновить сайт

Работаем в локальной папке проекта: `C:\Репетиторство\Сайты_для_репов\Настя_русс`

После правок выполни в этой папке:

```
git add .
git commit -m "описание изменений"
git push
```

GitHub Pages задеплоит изменения автоматически (обычно за 1–3 минуты). Проверить статус сборки можно здесь: https://github.com/Sashka350/Sashka350.github.io/actions

## Первая заливка (инфо на будущее)

Если проект нужно залить заново (например, на новый аккаунт):

```
git init
git branch -M main
git add .
git commit -m "Initial commit"
gh repo create NAME --public --source . --remote origin --push
gh api --method POST repos/USERNAME/NAME/pages -f build_type=legacy -f "source[branch]=main" -f "source[path]=/"
```

## Настройка GitHub Pages

Страница подключена через **Settings → Pages**: ветка `main`, каталог `/` (весь репозиторий — сайт).

## Что исключено из репозитория (.gitignore)

- `web_nastia/` — отдельный проект (собственный git-репозиторий)
- Экспорт страницы отзывов с Profi.ru (`*profi.ru*`, `*_files/`)
- Текстовые заметки (`*.txt`)
