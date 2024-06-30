# Клиент-серверное приложение о машинах

Проект представляет клиент-серверное приложение о машинах и их владельцах. В основе проекта лежит RestAPI для взаимодействия сервера с БД(`PostgreSQL`). Реализованы миграции через библиотеку `Goose`. Использовал библиотеку `Gin` для взаимодействия с серверной частью приложения. API задокументировал при помощи `Swagger` (`OpenAPI 2.0`). Также реализовано mock-тестировние.

Для запуска нужно создать файл `.env` в корне приложения с несколькими переменными окружения.

Пример переменных:

* POSTGRES_USER=postgres
* POSTGRES_PASSWORD=postgres
* POSTGRES_HOST=localhost
* POSTGRES_PORT=5432
* POSTGRES_DB=postgres


Для инициализации документации выполнить следующие команды

```

//go install github.com/swaggo/swag/cmd/swag@v1.8.12
//swag init -g cmd/main.go --parseDependency --parseInternal -d ./,internal/db,pkg/handlers - to generate docs

```
