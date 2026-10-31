# Публикация в GitHub и GitVerse

## 1. Создайте два пустых репозитория

Используйте одинаковое имя: `LR9-POP3-IMAP`.

- GitHub: создайте новый Public repository без README, .gitignore и лицензии.
- GitVerse: создайте новый репозиторий без автоматической генерации файлов.

Скопируйте HTTPS URL каждого репозитория. URL будет выглядеть примерно так (это примеры формата, не реальные адреса):
- `https://github.com/ВАШ_ЛОГИН/LR9-POP3-IMAP.git`
- `https://gitverse.ru/ВАШ_ЛОГИН/LR9-POP3-IMAP.git`

## 2. Установите Git, если он ещё не установлен

В Windows CMD:

```cmd
git --version
```

Если команда не найдена, установите Git for Windows с официального сайта https://git-scm.com/download/win, затем откройте новое окно CMD.

## 3. Откройте папку проекта

Распакуйте `LR9-POP3-IMAP.zip`, например в `C:\work\LR9-POP3-IMAP`, затем:

```cmd
cd C:\work\LR9-POP3-IMAP
```

## 4. Инициализируйте локальный Git-репозиторий

```cmd
git init
git branch -M main
git add .
git commit -m "Добавлены материалы лабораторной работы №9"
```

Если Git попросит имя и email, задайте их:

```cmd
git config --global user.name "Гамбердов Сулайм Исаевич"
git config --global user.email "ВАШ_EMAIL"
```

Затем повторите `git commit`.

## 5. Отправьте один и тот же проект на оба хостинга

Подставьте реальные URL, скопированные из ваших репозиториев:

```cmd
git remote add github https://github.com/ВАШ_ЛОГИН/LR9-POP3-IMAP.git
git remote add gitverse https://gitverse.ru/ВАШ_ЛОГИН/LR9-POP3-IMAP.git
git push -u github main
git push -u gitverse main
```

При запросе авторизации используйте браузерный вход или персональный токен, если площадка его запросит. Не отправляйте токены и пароли в чат.

## 6. Создайте релиз на каждом хостинге

После push откройте репозиторий на сайте и создайте Release/Релиз:
- Tag: `v1.0.0`
- Title: `Лабораторная работа №9 — POP3/IMAP`
- Description: `Отчёт, презентация и исходные материалы лабораторной работы №9.`

Прикрепите отдельными файлами из каталога `release/`:
- `report.md`
- `report.docx`
- `report.pdf`
- `presentation.md`
- `presentation.pdf`
- `presentation.html`
- `presentation.pptx`
- `source_materials.zip`

## 7. Что прислать мне после публикации

Пришлите две ссылки на репозитории и две ссылки на релизы. Я проверю, что структура и файлы доступны.
