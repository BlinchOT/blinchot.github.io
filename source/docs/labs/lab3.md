# Лабораторная работа №3: CI/CD для статического сайта

## Цель работы

Настроить непрерывную интеграцию и доставку (CI/CD) для статического сайта на MkDocs с использованием платформы SourceCraft и GitHub Actions.

## Задание

1. Реализовать автоматическое развертывание сайта на платформе SourceCraft.
2. Реализовать автоматическое развертывание этого же сайта на GitHub Pages с помощью GitHub Actions.
3. В рамках одного локального репозитория настроить два удалённых репозитория (sourcecraft и origin).
4. Предоставить четыре ссылки: на сайт и репозиторий в SourceCraft, на сайт и репозиторий на GitHub.

## Выполненные действия

### SourceCraft

1. Зарегистрировался на SourceCraft и создал публичную организацию `2212`.
2. Создал публичный репозиторий `mkdocs0902`.
3. Создал персональный токен доступа (PAT) с правами Maintainer.
4. Добавил удалённый репозиторий SourceCraft в локальный проект
5. Настроил файлы `.sourcecraft/sites.yaml` и `.sourcecraft/ci.yaml` для автоматического деплоя при пуше в ветку `main`.
6. Выполнил пуш в SourceCraft: `git push sourcecraft main`.

### GitHub Actions

1. Создал файл `.github/workflows/pages.yml` для автоматической сборки и публикации сайта.
2. Настроил GitHub Pages в репозитории `BlinchOT/Lr3-2` на использование GitHub Actions.
3. Выполнил пуш в GitHub: `git push origin main`.
4. GitHub Actions автоматически собрал сайт и опубликовал его на GitHub Pages.

## Настройки репозиториев

### Настройки GitHub

- Репозиторий: `BlinchOT/Lr3-2`
- GitHub Pages включен, публикация через GitHub Actions
- Workflow-файл: `.github/workflows/pages.yml`
- Права для GITHUB_TOKEN: `contents: write` (добавлено в workflow)

### Настройки SourceCraft

- Организация: `2212`
- Репозиторий: `mkdocs0902`
- Токен с правами Maintainer
- Конфигурационные файлы: `.sourcecraft/sites.yaml`, `.sourcecraft/ci.yaml`
- Ветка для публикации: `release`

## Ссылки на результат

| Платформа | Сайт | Репозиторий |
|-----------|------|-------------|
| SourceCraft | [2212.sourcecraft.site/mkdocs0902](https://2212.sourcecraft.site/mkdocs0902) | [sourcecraft.dev/2212/mkdocs0902](https://sourcecraft.dev/2212/mkdocs0902) |
| GitHub Pages | [blinchot.github.io/Lr3-2](https://blinchot.github.io/Lr3-2) | [github.com/BlinchOT/Lr3-2](https://github.com/BlinchOT/Lr3-2) |

## Выводы

В ходе работы я настроил CI/CD для статического сайта на двух платформах: SourceCraft и GitHub Pages. Автоматическая сборка и деплой происходят при каждом пуше в ветку `main`. Это позволяет быстро обновлять сайт без ручных операций.