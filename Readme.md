# Инструкция по работе с Git и удалёнными репозиториями

## Что такое Git?
***Git*** - это одна из реализаций распределённой системы контроля версий, поддерживающие как локальные, так и удалённые репозитории. Самая популярная реализация Git - это [GitHub](https://github.com)

## Подготовка репозитория
Для создания репозитория используется команда *git init*. Для этого необходимо открыть в терминале папку с будущим репозиторием и там написать *git init*

## Создание коммитов

### Выполнение коммита
Для того, чтобы выполнить коммит используется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать *git commit -m "<сообщение к коммиту>"*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!!***

### Добавление файла к коммиту
Для добавления файла к коммиту используется команда *git add*. Для этого в терминале с папкой-репозиторием необходимо написать *git add <название файла>*.

## Журнал изменений
Для просмотра истории коммитов используется команда *git log*. Для этого в терминале с папкой-репозиторием пишем *git log*. В показанном журнале обязательно будут:
* Хеш(номер) коммита
* Дата и время коммита
* Автор коммита
* Текст сообщения к коммиту

## Перемещение между коммитами
Для перещения между коммитами используется команда *git checkout*. Для этого в терминале с папкогой-репозиторием необходимо написать *git checkout <хеш коммита>*. Хеш коммита можно взять из истории коммитов, про которую было рассказано в предыдущем пункте

## Ветки в Git

Веток может быть неограниченное количество.

### Создание веток
Для создания новой ветки используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <название ветки>*. Название ветки должно быть ***УНИКАЛЬНО***!

### Просмотр списка веток
Для просмотра списка веток используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *giit branch* и Вы увидите список всех существующих веток. Зелёным цветом и символом **звёздочка** будет обозначена текущая актуальная ветка.

### Перемещение между ветками
Для перемещения между ветками используется команда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <название веткки*. Ветка ***ОБЯЗАТЕЛЬНО ДОЛЖНА СУЩЕСТВОВАТЬ!!!***. 

## Слияние веток и разрешение конфликтов

Для слияния веток используется команда git merge <имя ветки>
Для решения конфилитков можно в редатоктере принять входящее изменение , оставить предыдущее изменение , оставить оба изменения , либо отредактировать вручную

### Перемещение между ветками
Для перемещение между ветками используется команда git checkout branch 

## Удаление веток 

Для удаления веток используется команда git branch -d <имя ветки>

## Работа с Github

Чтобы создать репозиторий, на сайте [github.com](github.com) в личном кабинете нажимаем кнопку New repository

Чтобы перенести репозиторий в VS Code , нужно скопировать ссылку репозитория , использовать команду git clone <ссылка на репозиторий> и перейти в нужную папку репозитория командой cd <имя папки>. Желательно при работе создать новую ветку командой git branch <имя папки> и перейти в нее командой git branch checkout <имя созданой папки>

После работы с репозиторием , нужно отправить измененую локальную копию обратно на GitHub. Для этого выполняется команда git push origin master.

Если работа велась на самой платформе github , то чтобы те измененияя перенести в локальную копию используется команда git pull origin master

Для того чтобы предложить изменения в репозитории другого пользователя платформы , необходимо клонировать его репозиторий , внести изменения , выгрузить измененный репозиторий и предложить pull request

