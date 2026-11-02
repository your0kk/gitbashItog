# Памятка по Git

Команды выполняются в Git Bash из папки репозитория.

## Подготовка

```bash
git switch master
git pull --ff-only
git switch -c docs/my-change
```

Перед переключением ветки сохраните или закоммитьте текущие изменения.

## Сохранение правок

После редактирования файлов проверьте изменения:

```bash
git status
git diff
git add README.md
git commit -m "docs: update readme"
git push -u origin docs/my-change
```

В `git add` указывайте именно те файлы, которые хотите включить в коммит. Затем откройте Pull Request из своей ветки в `master` на GitHub, проверьте вкладку Files changed и выполните слияние.
