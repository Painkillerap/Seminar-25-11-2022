# Инструкция по работе с Git

## Что такое Git?
Git - это наиболее популярная реализация распределенной системы контроля версий.

В Git каждая рабочая копия кода сама по себе является репозиторием. Это позволяет всем разработчикам хранить историю изменений в полном объеме.

Разработка в Git ориентирована на обеспечение высокой производительности, безопасности и гибкости распределенной системы.

## Подготовка репозитория
Для создания репозитория в папке предполагаемого репозитория необходимо написать команду *git init*.
Для этого в терминале с открытой папкой-репозиторием необходимо написать *git init*.
 
## Добавление файлов к коммиту
Для добавления файлов к коммиту используется команда *git add*.
Для того, чтобы добавить файл к новому коммиту необходимо в терминале с открытой папкой-репозиторием написать *git add <имя файла>*.

## Создание коммитов 
Для создания коммитов используется команда *git commit*.
Для 'этого в терминале с открытой папкой-репозиторием необходимо написать *git commit -m "<сообщение к коммиту>"*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Журнал изменений
Для просмотра истории изменений используется команда *git log*.
Для этого в терминале с открытой папкой-репозиторием необходимо написать *git log*.

## Перемещение между коммитами
Для перемещения между коммитами используется команда *git checkout*. 
Для этого в терминале с папкой-репозиторием необходимо написать
*git checkout <номер коммита>*. Номера коммитов можно посмотреть в истории коммитов, описанной в предыдущем пункте.

## Ветки в Git
### Просмотр списка веток
Для просмотра списка веток используется команда *git branch*.
Для 'этого в терминале с открытой папкой-репозиторием необходимо написать *git branch*
### Переход между ветками
Для перемещения между ветками используется команда *git checkout*.
Для этого в терминале с папкой-репозиторием необходимо написать
*git checkout <название ветки>*.
### Создание новой ветки
Для создания новой ветки используется команда *git branch*.
Для 'этого в терминале с открытой папкой-репозиторием необходимо написать *git branch <название ветки>*.

## Слияние веток и разрешение конфликтов
Для слияния веток между собой используется команда *git merge*. 
Для этого в терминале с папкой-репозиторием необходимо написать
*git merge <название сливаемой ветки>*. Для разрешения конфликтов при выполнении слияния, необходимо отредактировать конфликтующий файл и удалить все разделители конфликта. После разрешения конфликта необходимо ***СОХРАНИТЬ*** файл, выполнить команду *git add* и команду *git commit*.

## Удаление веток
Для удаления ветки используется команда *git branch -d*.
Для этого в терминале с открытой папкой-репозиторием необходимо написать *git branch -d <название ветки>*.

## Работа с удаленным репозиторием
### Подключение к репозиториям
Для подключения к репозиторию используется команда *git remote*.
Для этого в терминале с открытой папкой-репозиторием необходимо написать *git remote*.
### Удаленное подключение к репозиториям
Для удаленного подключения к репозиторию используется команда *git clone*.
Для этого в терминале с открытой папкой-репозиторием необходимо написать *git clone < адрес репозитория>*. Два наиболее простых способа доступа к удаленному репозиторию: протоколы HTTP и SSH.

### Извлечение из удаленного репозитория
Для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым используется команда *git pull*.
Для этого в терминале с открытой папкой-репозиторием необходимо написать *git pull*.
### Выгрузка в удаленный репозиторий
Для выгрузки содержимого локального репозитория в удаленный репозиторий используется команда *git push*.
Для этого в терминале с открытой папкой-репозиторием необходимо написать *git push*
## Дополнительно
Также необходимые команды которые пригодятся:
* *git config* - для отображения конфигурации файла.
* *git status* - это функция, анализирующая два входных набора данных и отображающая различия между ними.
* *git diff* - для отображения состояния рабочего каталога и раздела проиндексированных файлов, а также файлов, удаленных из индекса Git.
* *git revert* - для отмены, но принцип ее действия отличается от привычной отмены изменений. Вместо удаления коммита из истории проекта эта команда отменяет внесенные в нем изменения и добавляет новый коммит с полученным содержимым.
* ## Заключение
Это минимальная инструкция по Git, в последующем ее необходимо дополнять другими материалами, в том числе, теми которые будут при совместной работе с Git.
