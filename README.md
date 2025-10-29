# Search generic Emails

## Назначение
Инструмент решает задачу сбора имейлов со списка сайтов

## Установка
Склонируем в созданную директорию и поставим зависимости в окружение
```sh
mkdir ~/Parser && cd ~/Parser && git clone https://github.com/Rickert155/genericEmail && cd genericEmail
```

```sh
python3 -m venv venv && ./venv/bin/pip install -r package.txt && ./venv/bin/pip freeze
```

## Режим отладки
Можно запускать парсер в режиме отладки. Для этого необходимо указкать параметр --debug и указать домен
```sh
python3 Generics.py --debug domain.com
```

## Сбор имейлов
В директорию Base необходимо добавить базу с доменами в формате csv. Название не имеет значение. Колонки, обязательные:

----------------
|Domain|Company|
----------------

Парсер будет обходить список доменов и писать результат в директорию Result/
