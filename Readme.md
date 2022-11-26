q# Инструкция по работе с git

## Что такое Git?
Git - это наиболее популярная реализация распространенной системы контроля версий. 

## Подготовка к работе в репозитории. Начало работы
Чтобы начать рабоqgit ту в Git, надо в левом верхнем углу нажать на "файл" и в появившемся списке выбрать "открыть файл" или "открыть папку". Если интересующий файл еще не создан, то в выбранной папке нужно будет создать файл ("файл" и "создать файл"(обязательно при создании указать тип файла). Когда интересующий файл будет создан и открыт через гит, то надо набрать *git init*. Эта команда положит начало отслеживанию изменений работы файла в Git.

## Создание изменений и сохранение изменений
После того, как в файле были совершены необходимые изменения надо нажать на сочетание клавиш *Ctrl +S*. Это сохранит изменения.

## Журнал изменений
Для просмотра истории изменений используется команда *git log*. Для этого в терминале с папкой репозиторием необходимо набрать *git log*.

## Создание коммитов
Для создания коммитов используется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать команду *git commit - m,сообщение к коммиту
*. Сообщение к коммину писать **ОБЯЗАТЕЛЬНО**
## Добавление файлов к коммиту
Для добавления файлов к коммиту используется команда *git add*. Для того, чтобы добавить файл к новому коммиту необходимо в терминате св открытой папкой-репозиторием написать *git add* <имя файла>*.

## Пермещение между сохранениями
Для перемещения между коммитами используется команда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git chtckout <номер коммита>*. Номера коммитов можно посмотреть в истории коммитов, описанной в предыдущем пункте

## Ветки в Git
Под веткой принятой понимать независимую последовательность коммитов в хронологическом порядке. Имя основной ветки по умолчанию *master*. Чтобы создать новую ветку надо набрать в терминале команду *git branch название ветки*. Чтобы переути на другую ветку надо ввести команду в терминал *git checkout название ветки*. 

## Просмотр списка веток
Для просмотра списка существующих веток надо набрать *git branch*. Для этого надо сделать в терминале в папке-репозиториии необходимо написать *git branch*

## Слияние веток 
Для того, чтобы слить ветки, надо вначале зайти в главную ветку. Эту в ту, с которой будем сливать другие ветки. Находясь на главной ветке, в терминале надо ввести команду *git merge <название ветки>

## Разрешение конфликтов 
При попытке некорректного слияния (когда в обоих ветках шли изменения в одном и том же месте и Git не знает, какая версия верная), Git останавливает выполнение команды, чтобы было возможно разрешить конфликт. Решить конфликт можно двумя способами: вручную разрешить файловых конфликт (для этого надо лично изменить файлы, с которыми возникли проблемы) или выбрать наиболее подходящий файл, отказавшись от другого.

## Удаление веток 
Для удаления используется в терминале команда  *git branch - d <название ветки>. Нельзя удалить ветку, если в ней находишься. Нельзя удалить ветку, у которой несохранены изменения.
