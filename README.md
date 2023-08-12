BookBuddy - Телеграм бот для удобного чтения книг

Этот Telegram-бот предоставляет возможность добавлять и удалять книги из личной библиотеки, а также читать их в удобном виде. Изначально в библиотеке присутствует книга "Марсианские Хроники". Для добавления собственной книги, просто отправьте её в чат в виде текстового файла (.txt).

При чтении книги можно добавлять закладки, нажав на кнопку текущей страницы. Закладки видны только для активной книги.

Команды:

    /start - запуск бота.
    /help - справка.
    /continue - продолжение чтения.
    /books - перечень книг.
    /bookmarks - закладки.

Для хранения данных бот использует базу PostgreSQL.
Зависимости

Python 3.8+
aiogram 3.0.*
psycopg2 2.9.6
python-dotenv 1.0.0
requests 2.31.0

Установка

    Клонирование репозитория:

bash

git clone [Ссылка на репозиторий]

    Создание виртуального окружения и установка пакетов:

bash

python3.8 -m venv env
source env/bin/activate
pip install -r requirements.txt

    Заполните файл .env.

    Запуск:

bash

python bot.py

Примечания

    При каждом запуске бота данные из базы удаляются и база заново инициализируется. Это связано с функцией setup_db. Если необходимо сохранить данные, закомментируйте вызов этой функции в bot.py.

    Для тестирования бота добавлены примеры книг в папке books/.
