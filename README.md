# Проект интернет-магазина

## Структура проекта
``` 
django_hw/
├── catalog/                          # Основное приложение магазина
│   ├── migrations/                   # Миграции базы данных
│   ├── templates/catalog/            # Шаблоны приложения
│   │   ├── contacts.html             # Страница контактов
│   │   └── home.html                 # Главная страница
│   ├── __init__.py
│   ├── admin.py                      # Настройки админки
│   ├── apps.py                       # Конфигурация приложения
│   ├── models.py                     # Модели данных (товары, категории)
│   ├── tests.py                      # Тесты
│   ├── urls.py                       # Маршруты приложения
│   └── views.py                      # Представления
│
├── config/                           # Основная конфигурация проекта
│   ├── __init__.py
│   ├── asgi.py                       # ASGI-конфигурация
│   ├── settings.py                   # Настройки Django
│   ├── urls.py                       # Главный файл URL-маршрутов
│   └── wsgi.py                       # WSGI-конфигурация
│
├── static/                           # Статические файлы
│   ├── css/
│   │   └── bootstrap.min.css         # Bootstrap CSS
│   └── js/
│       └── bootstrap.bundle.min.js   # Bootstrap JS
│
├── manage.py                         # Управление проектом
├── poetry.lock                       # Фиксированные зависимости Poetry
├── pyproject.toml                    # Конфигурация Poetry и зависимостей
├── README.md                         # Документация
└── .gitignore                        # Игнорируемые файлы Git
```

## Установка и запуск

### 1. Клонирование репозиторя
```
git clone https://github.com/Aleksei-Pavlovskii/django_hw.git>
cd django_hw
```

### 2. Установка зависимостей
Проект использует Poetry для управления зависимостями.

Установите Poetry, если ещё не установлен:

```
pip install poetry
```
Установите зависимости проекта:
```
poetry install
```


### 3. Запуск сервера
``` 
poetry run python manage.py runserver
```

### 🌐 Основные страницы
+ Главная страница (`/`) — `home.html`

+ Контакты (`/contacts/`) — `contacts.html`

+ Админ-панель (`/admin/`) — доступна после создания суперпользователя