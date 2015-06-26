# Тестовое задание для соискателя на должность Frontend | Android разработчика

Нужно сделать CRUD интерфейс для базы данных роботов.

Данный проект построен на архитектуре REST API и в нем доступны следующие вызовы

### Получение всех роботов

1. Url: http://frontend.test.pleaple.com/api/robots
2. Method: GET

Пример запроса:
curl -i -X GET http://frontend.test.pleaple.com/api/robots

### Поиск робота
1. Url: http://frontend.test.pleaple.com/api/robots/search/:name
2. Method: GET
3. Data: {name: "Название робота"}

Пример
curl -i -X GET http://frontend.test.pleaple.com/api/robots/search/Astro

### Получение робота по ID
1. Url: http://frontend.test.pleaple.com/api/robots/:id
2. Method: GET
3. Data: {id: "ID робота"}

Пример
curl -i -X GET http://frontend.test.pleaple.com/api/robots/3

### Добавление робота
1. Url: http://frontend.test.pleaple.com/api/robots
2. Method: POST
3. Data: {"name":"Название робота","type":"Тип робота","year":Год создания}

Пример
curl -i -X POST -d '{"name":"C-3PO","type":"droid","year":1977}' http://frontend.test.pleaple.com/api/robots

### Редактирование робота
1. Url: http://frontend.test.pleaple.com/api/robots
2. Method: PUT
3. Data: {"name":"Название робота","type":"Тип робота","year":Год создания}

Пример
curl -i -X PUT -d '{"name":"ASIMO","type":"humanoid","year":2000}' http://frontend.test.pleaple.com/api/robots/4

### Удаление робота
1. Url: http://frontend.test.pleaple.com/api/robots/:id
2. Method: DELETE
3. Data: {id: "ID робота"}

Пример
curl -i -X DELETE http://frontend.test.pleaple.com/api/robots/4

## Для Frontend разработчика

#### Сам интерфейс нужно разработать на Backbone Marionette (http://marionettejs.com/) в оформлении можно использовать bootstrap

Результат работы должен оказаться в GIT репозитории

## Советы
1. Не забываем работать с репозиторием. Для git является хорошей практикой делать много коммитов(commit) и меньше пушей (push)
2. Не забываем комментировать код. Не нужно фанатизма, достаточно описание функций и сложных участков кода внутри функций.
3. Не тратьте время на дизайн, нужна только чистая верстка и код
4. Если вам кажется что потратили уже много времени, вполне можете выложить то что уже есть. Возможно этого будет достаточно.

## Полезные материалы
1. Документация на русском по backbone http://backbonejs.ru/
2. Документация на русском по marionette http://instanceof.pro/marionettejs.ru/
3. Хороший пример архитектуры https://github.com/an2323/listcontacts/tree/64cea59785e7f3464c1d651d2547970e65e3bad2
4. Дополнитеоьный материал http://shustov.su/blog/javascript/backbone-marionette

Если будут вопросы пишите. По возможности помогу.

## Удачи вам в выполнении этого задания

## Для Android разработчика

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
