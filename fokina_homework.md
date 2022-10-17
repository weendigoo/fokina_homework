# Семинар 1

## Руководство по использованию git

* *git init* - добавление репозитория.
* *git add <имя файла>* - добавление файла к списку отслеживаемых.
* *git commit* -m "комментарий" - добавление "точки сохранения" и присвоение ей определённого статуса.
* *git log* - открытие журнала изменений.
* *git log --graph* - отображение графика работы с репозиторием.
* *git diff* - отображение разницы между версиями проекта.
* *git checkout <имя ветки>* - переход на ветку <имя ветки>
* *git branch <имя ветки>* - создание ветки <имя ветки>
* *git branch* - проверка списка всех веток и отображение текущей ветки. 
* *git branch -d <название ветки>* - удаление ветки <название ветки>
* *git merge <название ветки>* - слияние ветки <название ветки> с веткой master
* *clear* - очистка видимой зоны терминала
* *git cd <folder name>* - переход к папке <folder name>

## Основной алгоритм работы с git
1. добаление изменений
2. сохранение файла
3. добавление комита/комментария
4. продолжение работs


# Семинар 2

## Создание веток

* Для создания новой ветки импользуется команда *git branch <имя_ветки>*.
* Для ознакомления с уже существующими в репозитории ветками используется команда *git branch*

## Слияние веток

* При слиянии веток необходимо находиться в базовой ветке, а в команде *merge* указывать название сливаемой ветки.

* *git merge <имя ветки>* - команда осуществляющая слияние.



## Возникновение и решение конфликтов

Если изменения в сливаемых ветках затрагивают общую рабочую ветку, это приводит к конфликту при слиянии.

Необходимо выбрать наиболее оптимальный вариант из предложенных версий. 
Однако, если изменения затрагивают различные области проекта слияние происходит автоматически.


# Семинар 3

## Работа с удалёнными репозиториями


### Работа с собственным удалённым репозиторием 

* *git branch -M <master/main>* - добавление ветки <master/main> в удалённый репозиторий
* *git remote add origin <link of remote reposytory>* - синхронизация удалённиго и локального репозиориев
* *git push -u origin master* - проведение аутентификации в браузере (при подключении с нового устройства)
* *git push* - отправка изменений/наиболее актуальной версии из локального в удалённый репозиторий (если акаунты VScode и GitHub уже синхронизированны) 
* *git pull* - отправка изменений/наиболее актуальной версии из удалённого в локалььный репозиторий (если акаунты VScode и GitHub уже синхронизированны) 


### Работа с удалённым репозиторием другого пользователя

Для работы с удалённым репозиторием другого пользователя:

1. Копировать ссылку/адрес на тот репозиторий пользователя, с которым вы планируете работать.
2. Добавить репозиторий на ваше устройство. Для этого вставьте ссылку/адрес репозитория в строку "добавление репозитория" предварительно выбрав "импортировать из GitHub".
3. Создать собственную ветку для внесения изменений во избежание конфликтов при слиянии.
4. Внесение ваших изменений и создание коммитов.

Для отправки изменений владельцу удалённого репозитория:

1. Выбрать команду "fork" в меню GitHub.
2. Заполнить необходимые поля и созать свой "fork"
3. Отправить вашу версию проекта его владельцу используя интерфейс GitHub.