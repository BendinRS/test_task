# Тестовое задание

## Постановка задачи

задача для плейбука
+ - сбор фактов и вывод на дебаг. Из фактов выбираем нужные (хостнейм, ип итд)  
+ - анализируем сервисы которые есть в systemctl, смотрим статусы, версии - выдаем на экран  
+ - ресурсы системы - память , цпу - всего, занято, свободно  
+ - диски, точки монтирования, занятость  
+ - порты в состоянии Listen - какие сервисы их слушают  
+ - пользователи у которых есть шелл  
+ - крон скрипты  

Генерация репорта через jinja2


## Ход работы

+ Разворачивается ВМ
+ Запускается роль ансибл. [Основной плей](./test/tasks/main.yml)
+ Вывод информации отображается в ходе работы vagrant
+ Так же файл со сбором фактов после выполнения vagrant можно найти в папке с именем хоста

Пример файла вывода сбора фактов:
![Checksystem](https://i.ibb.co/55z8DHm/12345.png)

