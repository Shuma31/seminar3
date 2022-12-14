# **Инструкция по работе с Git**

![Эмблема Git](Git.jpg)

## Инициализация репозитория 

***Для инициализации (создания) репозитория используется команда:***

    git init 

## Проверка состояния репозитория

***Чтобы проверить текущее состояние репозитория используется команда:***

    git status

## Добавление в индекс
***Для добавления содержимого рабочей директории в индекс - используется команда:***

    git add

## Фиксация изменений
***Для того, чтобы зафиксировать изменения в репозитории, находящиеся в индексе - используем команду:*** 

    git commit -m "message"

## Добавление и фиксация в одной команде
***В Git добавить и зафиксировать в одной команде - используется:***

    git commit -a

## Доступ к истории
***Для того, чтобы получить доступ к истории депозитория используется команда:***

    git log

 ***Вывод истории в более компактном виде:***


    git log --oneline

## Переход к старому состоянию проекта
***Чтобы вернуться к последнему коммиту используем команду:***

    git checkout

## Вычисление разницы
***Для вычисления разницы между любыми двумя коммитами используется команда:***

    git diff


## Ветвление
Ветвление — это основная концепция системы управления версиями, которая позволяет разделять работу по разным ветвям, чтобы мы могли свободно работать с исходным кодом, не затрагивая чью-либо работу или фактический код в основной ветви.

***Для того, чтобы посмотреть какие ветки у нас есть и на какой ветке мы находимся, необходимо ввести команду:***

    git branch

## Создание новой ветки
***Для создания новой ветки используется команда:***

    git branch <branch_name>


## Слияние веток

Слияние веток – это перенос изменений с одной ветки на другую. Для этого надо перейти на ветку master — ту ветку, в которую сливают изменения.

***Чтобы слить указанную ветку в текущую ветку необходимо использовать команду:***

    git merge <name_branch>


## Разрешение конфликтов
Очень часто во время слияния веток оказывается, что наши изменения удаляют или переписывают информацию в уже существующих файлах. Такая ситуация называется конфликтом. Git останавливает выполнение слияния, пока мы не разрешим конфликт.

 Существует два способа разрешать конфликты:
1. Разрешить конфликт вручную. Тогда мы можем самостоятельно изменить конфликтные файлы, сделав их такими, какими мы хотим их видеть.
2. Просто выбрать один из вариантов, которые предлагает программа, а именно:
     * Оставить вариант, который был в master
     * Подтвердить входящие изменения и удалить то, что было в master
     * Подтвердить оба варианта


## Удаление ветки 
***Для того, чтоб удалить ветку, нужно ввести команду:***

    git branch -d <name_branch>

## Добавление изображения в текст
Для того, чтобы добавить картинку в текст, необходимо нужую картинку поместить в папку, где находится файл репозитория. Так как изображение не является текстовым файлом, то git может не корректно работать с данным файлом, поэтому нужно, чтоб git не отслеживал нашу картинку. Для этого в репозитории необходимо создать файл, который git будет игнорировать и в этот файл записать имя нашего изображения. 

    .gitignore

## Удалённые репозитории
Удалённые репозитории нужны для совместной работы.

