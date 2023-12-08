# kittygram_final
Социальная сеть для обмена фотографиями любимых питомцев. Котограм воплоти!

# Kittygram
### Описание
Сайт - на котором вы можете лицезреть замечательных котиков. Но это не всё! Вы можете добавить своих котиков и рассказать о них подробнее. Например, можно указать кличку, цвет окраса и даже фото вашего питомца! Покажи котейку миру!

### Технологии
Python 3.9 
Django 3.2.3

### Запуск проекта в dev-режиме
- Выпоните клонирование кода приложения с GitHub:
```
git clone git@github.com:Ваш_аккаунт/kittygram_final.git
```
- Перейдите в директорию backend-приложения проекта:
```
cd kittygram_final/backend/
```
- Установите и активируйте виртуальное окружение:
```
python3 -m venv venv
```
```
source venv/bin/activate
```
- Установите зависимости из файла requirements.txt:
```
pip install -r requirements.txt
```
- Выполните миграции:
```
python manage.py migrate
```

- Выполните автоматический запуск по инструкции, использовав Docker Compose, из директории, где находится файл docker-copmose.yml:
- Запуск Docker Compose:
```
docker compose up 
```
- Перезапустить Docker Compose после изменений можно так:
```
docker compose stop && docker compose up --build 
```


### Автор
Владислав Т
https://github.com/Trishkin32
