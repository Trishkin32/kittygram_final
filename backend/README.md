# kittygram_final
Социальная сеть для обмена фотографиями любимых питомцев. Котограм воплоти!

# Kittygram
### Описание
Сайт - на котором вы можете лицезреть замечательных котиков. Но это не всё! Вы можете добавить своих котиков и рассказать о них подробнее. Например, можно указать кличку, цвет окраса и даже фото вашего питомца! Покажи котейку миру!

### Технологии
Python 3.9 
Django 3.2.3


### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:
git clone git@github.com:Trishkin32/kittygram_final.git
cd kittygram_final/backend

Cоздать и активировать виртуальное окружение:
```
python3 -m venv env
```

* Если у вас Linux/macOS
  ```
    source env/bin/activate
  ```
    

* Если у вас windows
  ```
    source env/scripts/activate
```
```    
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:
```
pip install -r requirements.txt
```

Выполнить миграции:
```
python3 manage.py migrate
```

Запустить проект:
```
python3 manage.py runserver
```

### Как запустить проект в контейнере Docker:


Клонировать репозиторий и перейти в него в командной строке:
```
git clone https://github.com/Trishkin32/kittygram_final.git
```
cd kittygram_final/backend
```

Убедитесь, что Docker запущен.

Выполните сборку образа:
```
docker build -t kittygram_backend .
```

Запустите контейнер:
```
docker run --name kittygram_backend_container --rm -p 9000:9000 kittygram_backend
```

Выполните миграции в контейнере (в отдельном терминале):
docker exec kittygram_backend_container python manage.py migrate
Теперь вы можете отправлять запросы к api, например, создать пользователя. Пример POST-запроса к api/users/:

```
{
    "email": "user@mail.com",
    "username": "user",
    "password": "user_password"
}
```



### Автор
Владислав Т
https://github.com/Trishkin32
