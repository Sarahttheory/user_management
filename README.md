# User management

Данное приложение реализует авторизацию и регистрацию пользователей с различными ролями.
При авторизации пользователю предоставляется навигационная панель с кнопками, 
которые выводят данные из созданных таблиц в базе данных.

## Подготовка к использованию
- **Установка зависимостей:** Для начала убедитесь, что у вас установлены все необходимые зависимости, 
указанные в файле `composer.json`. Выполните команду `composer install` в корневой директории проекта.


- **Настройка базы данных:** Вам потребуется база данных для работы приложения.
Укажите параметры подключения к базе данных в файле `config/db.php`.


- **Применение миграций:** Выполните миграции, чтобы создать необходимые таблицы в базе данных. 
Для этого выполните команду `php yii migrate` в корневой директории проекта.


- **Заполнение тестовыми данными (опционально):** Если вы хотите заполнить таблицы тестовыми данными, 
выполните миграции с флагом `--migrationPath=@app/migrations/test`. Это создаст тестовых пользователей и 
другие данные для проверки функционала.

## Использование приложения
- **Регистрация и авторизация:** При первом запуске приложения вы можете зарегистрировать нового пользователя или использовать предварительно созданных тестовых пользователей для авторизации.


- **Навигационная панель:** После авторизации пользователю будет доступна навигационная панель с кнопками для доступа к различным разделам приложения.


- **Отображение данных:** При нажатии на кнопки в навигационной панели, приложение будет выводить данные из соответствующих таблиц в базе данных.


- **Роли и доступы:** Каждому пользователю в приложении присваивается определенная роль, например, "Admin" или "User". В зависимости от роли, пользователь может иметь доступ только к определенным разделам приложения.
