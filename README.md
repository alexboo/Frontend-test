# Тестовое задание для соискателя на должность  Android разработчика

Нужно сделать CRUD интерфейс для базы данных роботов.

Данный проект построен на архитектуре REST API и в нем доступны следующие вызовы

### Получение всех роботов

1. Url: http://help.flip.kz/robots/api/robots
2. Method: GET

Пример запроса:
curl -i -X GET http://help.flip.kz/robots/api/robots

### Получение робота по ID
1. Url: http://help.flip.kz/robots/api/robots/:id
2. Method: GET
3. Data: {id: "ID робота"}

Пример
curl -i -X GET http://help.flip.kz/robots/api/robots/1

### Добавление робота
1. Url: http://help.flip.kz/robots/api/robots
2. Method: POST
3. Data: {"name":"Название робота","type":"Тип робота","year":Год создания}

Пример
curl -i -X POST -d '{"name":"C-3PO","type":"droid","year":1978}' http://help.flip.kz/robots/api/robots

### Редактирование робота
1. Url: http://help.flip.kz/robots/api/robots/:id
2. Method: PUT
3. Data: {"name":"Название робота","type":"Тип робота","year":Год создания}

Пример
curl -i -X PUT -d '{"name":"C-3PO","type":"droid","year":1977}' http://help.flip.kz/robots/api/robots/1

### Удаление робота
1. Url: http://help.flip.kz/robots/api/robots/:id
2. Method: DELETE
3. Data: {id: "ID робота"}

Пример
curl -i -X DELETE http://help.flip.kz/robots/api/robots/7

#### В работе желательно использовать следующие технологии
1. MVP
2. JSON
3. Jackson mapper
4. http://loopj.com/android-async-http/
5. Activity
6. Fragment
7. Material Design

## Советы
1. Один экран с выводом и редактированием сущности
2. Обратить внимание на переворот устройства.

## Удачи вам в выполнении этого задания
