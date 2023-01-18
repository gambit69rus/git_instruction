# Инструкция для работы с git и удаленными репозиториями
## Что такое git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду git init в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)
## Создание коммитов
### Git add
Для добавления измений в коммит используется команда git add. Чтобы использовать команду git add напишите git add <имя файла>
### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда git status. Для этого необходимо в папке с репозиторием написать git status, и Вы увидите были ли измения в файлах, или их не было.
### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду git commit. Выполняется она так: git commit -m "<сообщение к коммиту>. Все файлы для коммита должны быть ДОБАВЛЕНЫ и сообщение к коммиту писать ОБЯЗАТЕЛЬНО.
## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда git checkout. Используется она в папке с пепозиторием следующим образом: git checkout <номер коммита>
## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда git log. Для этого достаточно выполнить команду git log в папке с репозиторием
## Ветки в Git
### Создание ветки
Для того, чтобы создать ветку, используется команда git branch. Делается это следующим образом в папке с репозиторием: git branch <название новой ветки>
## Слияние веток
Для того чтобы дабавить ветку в текущую ветку используется команда git merge
## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"
# Инструкция для работы с Markdown
## Выделение текста 
Чтобы выделить текст курсивом необходимо обрамить его звездочками (*) или знаком нижнего подчеркивания (_). Например, *вот так* или _вот так_. 

Чтобы выделить текст полужирным необходимо обрамить его двойными звездочками (*) или двойным знаком нижнего подчеркивания(__). Например, **вот так** или __вот так__.

Альтернативные способы выделения текста жирным или курсивом нужны для того чтобы мы могли совмещать оба этих способа. Например _текст может быть выделен курсивом и при этом быть **полужирным**_.
## списки
Чтобы добавить ненумерованные списки необходимо пункты выделить звездочкой (*) или знаком (+). Например вот так:
* Элемент 1
* Элемент 2
* Элемент 3
+ Элемент 4

Чтобы добавить нумерованные списки, необходимо пункты просто пронумеровать. Например вот так: 
1. Первый пункт
2. Второй пункт
## Работа с изображениями
Чтобы вставить изображение в текст, достаточно написать следующее:
![привет это пушок](dog.jpeg)
## Работа с таблицами
В чистом Маркдауне нет синтаксиса для таблиц, а в GFM есть.

первый столбец | второй столбец
---------------| ---------------
ячейка         | ячейка
ячейка         | ячейка

Для красоты можно и по бокам линии нарисовать:

| первый столбец| второй столбец|
| ------------- | ------------- |
| ячейка        | ячейка        |
| ячейка        | ячейка        |

Можно управлять выравниванием столбцов при помощи двоеточия.

|выравнивае слева|выравнивание по центру| выравнивание справа|
|:---------------|:--------------------:| ------------------:|
| ячейка         | ячейка               |     ячейка         |
| ячейка         | ячейка               |     ячейка         |
| ячейка         | ячейка               |     ячейка         |

Внутри таблиц можно использовать ссылки, наклонный, жирный или зачеркнутый текст.
## Цитаты
Чтобы записать цитату необходимо использовать (>) перед текстом. Например 
>Это цитата

В цитаты можно помещать всё что угодно, в том числе вложенные цитаты используя два знака (>>), например:
> ## Это заголовок
> 1.   Это первый уровень цитирования
>> 2.   Это второй уровень цитирования
>>> 3.   Это третий уровень цитирования

## Ссылки

Текст ссылки заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. 

[Например](htpp://exemple.com)

При создании сносной гиперссылки вместо целевого адреса используется вторая пара квадратных скобок, внутри которых помещается метка, идентификатор ссылки (id). В этом случае возможно определить идентификатор в любом месте документа:

Например [id]:

[id]:http://example.com/

