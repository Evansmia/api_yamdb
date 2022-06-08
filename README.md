# API_YaMDb
## REST API для сервиса YaMDb — базы отзывов о фильмах, книгах и музыке
### Авторы:
- Ilya Rogozin https://github.com/ilyarogozin
- Mia Evans https://github.com/Evansmia
- Vlad Pronko https://github.com/VladPronko
### Распределение задач в команде:
- Ilya Rogozin
>Всё, что касается управления пользователями (Auth и Users): система регистрации и аутентификации, права доступа, работа с токеном, система подтверждения через e-mail.
- Mia Evans
>Категории (Categories), жанры (Genres) и произведения (Titles): модели, представления и эндпойнты для них.
- Vlad Pronko
>Отзывы (Review) и комментарии (Comments): описание моделей, представлений, настройка эндпойнтов, определение прав доступа для запросов, рейтинги произведений.
### Технологии:
- Python
- Django
- DRF

# Как запустить проект:
- Клонировать репозиторий и перейти в него:
>git clone https://github.com/Evansmia/api_yamdb.git

>cd api_yamdb

- Cоздать и активировать виртуальное окружение:
>python3 -m venv env

>source venv/Scripts/activate  #для Windows
>source venv/bin/activate      #для Linux и macOS

- Установить зависимости из файла requirements.txt:
>python3 -m pip install --upgrade pip

>pip install -r requirements.txt

- Выполнить миграции:
>python3 manage.py migrate

- Для заполнения БД sqlite тестовыми данными:
>убедитесь, что вы находитесь в корневой папке проекта(где находится manage.py)
>запустите файл csv_to_db.py из консоли: python3 csv_to_db.py

- Запустить проект:
>python3 manage.py runserver

## Примеры запросов к API можно посмотреть по запросу:
http://127.0.0.1:8000/redoc/
