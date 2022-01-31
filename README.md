# Выполнение заданий #
Задание выполнено в рамках "Школы разработки".<br>
Ссылки на развернутые приложения:
- с ветки [develop](https://progerfour.github.io/Invoices/develop/)
- с ветки [master](https://progerfour.github.io/Invoices/master/)

## Что можно сделать с помощью данного веб-приложения? ##
1. На главной странице приложения просмотреть список счетов (накладных).
2. Выполнить создание, редактирование и удаление накладных.
3. Отфильтровать данные по значению выбранного поля (с использованием операции “равно”).
4. Для списка на главной странице приложения поддерживается полнотекстовый поиск по всем полям.
5. Для списка на главной странице приложения подерживается сортировка по одному полю в трех режимах: “по возрастанию”, “по убыванию”, “без сортировки”. Фильтрация, сортировка и поиск для списка на главной странице приложения работают совместно, т.е. в запросе  учитыватся всё, что выбрал пользователь.

## Что было использовано? ##
* Для получения списка накладных выполняются запросы к серверу на основе REST API.
* В качестве сервера для публикации REST API использован JSON Server.
* Сервер развернут на Heroku.
* Для выполнения запросов к серверу из приложения используется AJAX (средствами jQuery)

## Тестирование ##
* Было выполнено тестирование с помощью инструментов postman и fiddler (результаты в папке task_2).
* Для репозитория настроен серверный билд и Continuous Integration с использованием сервиса Travis CI
* Серверный билд запускается при каждом коммите в репозиторий.
* В процессе работы серверного билда запускаютя тестовые коллекции при помощи инструмента Newman.
* Билды, которые запущены с веток master и develop, инициируют автоматическое развертывание клиентского приложения на GitHub Pages, связанных с данным репозиторием.
