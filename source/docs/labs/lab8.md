# Лабораторная работа №8: Скрапинг и анализ текста

## Введение

В работе выполнен сбор данных с сайта news.itmo.ru с использованием методов веб-скрапинга. Собраны данные о новостях по ключевым словам «нейротехнологии» и «нейротехнологии и программирование».

## Цель работы

Освоить методы скрапинга данных из веб-страниц.

## Ход работы

1. Выполнен сбор общих данных о новостях (ID, название, дата, URL).
2. Для каждой новости собраны детальные данные (ID, название, дата, просмотры, текст, теги).
3. Данные сохранены в CSV-файлы.

## Структура данных

### Общий список (news_list.csv)
- Идентификатор новости
- Название новости
- Дата размещения
- URL

### Детальный список (news_content/detailed_news.csv)
- Идентификатор
- Название новости
- Дата размещения
- Количество просмотров
- Текст
- Теги

## Итоговые файлы

- [news_list.csv](https://github.com/BlinchOT/blinchot.github.io/blob/main/news_list.csv)
- [detailed_news.csv](https://github.com/BlinchOT/blinchot.github.io/blob/main/news_content/detailed_news.csv)

## Ссылка на Jupyter Notebook

[Ноутбук lab8](https://colab.research.google.com/drive/1p0eCnDsSsSdlbCOnxQDgVdLuc-6bNhPH?usp=sharing#scrollTo=Pzv_l6e1LjPv)