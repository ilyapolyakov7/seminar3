# **Инструкция по работе с Git**

![emblema git](git.png)

Git — система управления версиями с распределенной архитектурой. Система Git была изначально разработана в 2005 году Линусом Торвальдсом — создателем ядра операционной системы Linux.

## Инициализация репозитория

Для инициализации (создания) репозитория используется команда:

    git init

## Проверка состояния репозитория

Для проверки текущего состояния репозитория используется команда:

    git status

## Добавление версионности

Для добавления отслеживания изменений используется команда:

    git add <полное имя файла>

## Фиксация изменений

Для фиксации изменений используется команда:

    git commit

После этого откроется окно для ввода сообщения о создаваемом коммите.

Чтобы ввести сообщение в процессе создания коммита используется эта же команда с дополнительным функционалом:

    git commit -m "сообщение"

## Просмотр истории коммитов

Для просмотра истории коммитов используется команда:

    git log

Для просмотра логов в кратком виде используется та же команда с допольтельным функционалом:

    git log --oneline

Для просмотра всех логов вне зависимости от текущей версии используется та же команда с допольнительным функционалом:

    git log --all

## Переключение между версиями

Для переключения между ранее сохраненными версиями используется команда:

    git checkout <hash>

## Просмотр различий между коммитами

Для просмотра различий между текущим состоянием и последним закомиченным ипользуется команда:

    git diff

Для просмотра различий между двумя определенными версиями используется команда:

    git diff <hash1> <hash2>

## Ветвление

Ветвление означает, что вы отклоняетесь от основной линии разработки и продолжаете работу, не вмешиваясь в основную линию.

### Создание новой ветки

Для создания новой ветки используется команда:

    git branch <branch name>

### Команда слияния

Для того, чтобы влить ветку в текущую нужно использовать команду:

    git merge <merge name>

### Просмотр всех веток

Для просмотра существующих веток и на какой находимся, используется команда:

    git branch

### Переключение между ветками

Для переключения между ветками используется команда:

    git checkout <имя_ветки>

### Удаление веток

Чтобы удалить ветку используется команда:

    git branch -d <имя ветки>

### Конфликты при слиянии

Если одна и та же строка в разных версиях записана по-разному, то возникает конфликт. VSCode дает возможность какое изменение сохранить (входящее, существующее или оба).

## Удаленные репозитории

Удаленные репозитории нужны для совместной работы.
