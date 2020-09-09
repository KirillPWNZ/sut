## Отчет по проектно-технологической практике
Разработка изолированных приложений при помощи технологий контейнеризации на примере sql-сервиса с web доступом

Состав бригады:
  * Тарасов К.Е. - написание docker-compose файла
  * Пономарев Н.В. - поиск и подготовка образов БД и ui для администрации БД
  * Сергеев М.А. - работа с git и docker-hub

### Используемый стек
1. PostgreSQL для создания системы управления БД.
2. pgAdmin для удобного интерфейса администратора БД.
3. Docker+Docker Compose для контейнеризации приложений.

### Запуск проекта:
Находясь в директории с файлом docker-compose.yml:
```
sudo docker-compose up --build -d
```

### Проверка
1. Открыть браузер по адресу http://localhost:8080/ и дождаться загрузки web интерфейса pgAdmin.
2. Войти в систему, используя логин/пароль: 
```
admin@host.com/password
```
3. Создать БД, кликнув правой кнопкой по Server.
4. Ввести в поле Hostname во вкладке SQL 
```
pgsql-server
```
5. Ввести пароль 
```
password
```
