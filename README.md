*Инструкция по работе с GIT**

Данная иструкция составлена для помощи себе в дальнейшей работе с системой контроля версий.

## Что такое GIT


Система контроля версий Git была создана *Линусом Торвальдсом* для работы при создании ядра ОС Linux. На данный момент это самая популярная система контроля версий в мире.

## Создание репозитория

Для создания репозитория (говорят "инициализации") используется команда:

    git init

## Добавление коммитов

Для отслеживания версионности необходимо вначале добавить измененный файл (не забыть его сохранить) к отслеживанию, а затем зафиксировать изменения.

### Добавление версионности

Чтобы добавить файл к отслеживанию версионнности используется команда:

    git add <имя файла>

где <имя файла> - полное имя добавляемого файла с расширением.

### Создание коммита

Чтобы зафиксировать изменения используется команда:

    git commit -m "комментарий"

где "комментарий" - краткое описание изменений в этом коммите. Кавычки обязательны!

### Просмотр состояния

Чтобы просмотреть текущее состояние репозитория используется команда:

    git status

## Команды для просмотра журнала изменений

Чтобы просмотреть историю изменений используется команда:

    git log

Возможно использование параметра для просмотра истории в сокращенном виде:

    git log --oneline

## Команды для работы с коммитами

Для переключения между разными "сохранениями" используется команда:

    git checkout <хэш коммита>

где <хэш коммита> - специальный набор символов однозначно определяющий каждый коммит.

## Просмотр различий

Для просмотра различий между версиями используется команда:

    git diff

В таком виде будут показаны различия между текущим (незакоммиченным) состоянием репозитория и последним актуальным коммитом.

Либо можно использовать команду:

    git diff <хэш1> <хэш2>

Где <хэш1> <хэш2> - хэши сравниваемых коммитов.

## Создание веток

Для создания новой ветки используется команда:

    git branch <имя ветки>

## Переход между ветками

Для перехода на другую ветку исползуется команда:

    git checkout <имя ветки>

## Слияние веток

Для того, чтобы влить одну ветку в другую нужно перейти в ту ветку КУДА будем производить слияние и ввести команду:

    git merge <имя ветки из которой добавляем изменения>

## Удаление веток

Для удаления ветки используется команда:
    
    git branch -d branches
