## Описание формата разработки и поддержки решений  
Назначение: подготовка к проекту, проектная работа, разработка решений и проектной документации, внедрение, эксплуатация  
### 1. Папки репозитария:  
>**./BOOK** Для проектной и эксплутационной документации, книг, описаний  
>**./TOOL** Инструментарий  
>**./GOLD** Условия и результат оплаты  

### 2. Задачи:  
#### Правила присвоения имен задачам:  
Коротко обозначить: подсистему и функционал, и цель создания задачи

#### Правила создания первичного описания задачи:  
(1) Обозначить цели задачи  
>**0INF** = запрос на предоставление информации  
>**0REQ** = запрос на создание, разработку, выполнение работ  
>**1PRE** = подготовка к разработке, сбор исходных данных, систематизация, анализ, формирование требований и подготовительной документации  
>**2DOC** = разработка и правка документации, описаний, схем, книг, моделей...  
>**2DEV** = развитие (разработка), создание прототипа, разработка нового функционала  
>**3RED** = правки, модификации, изменения, оптимизация существующего функционала  
>**3TST** = тестирование прототипа, функционала, изменений, совместимости  
>**3END** = работы приостановлены или отменены  
>**4SUP** = осуществляется техподдержка (фиксация, диагностика и решение проблем в стабильной версии)  
>**4BUG** = исправление неточностей и небольших ошибок  
>**4RAT** = исправление серьезных ошибок и проблем (патч, заплатка)  
>**4ASK** = нужен ответ на вопрос или консультация  
>**5RUN** = тестовая эксплуатации  
>**LOOP** = похожая задача уже существует  
>**OK** = проверенная версия  
(2) Описание планируемого практического применения результата работ  
(3) Ссылки на проект  
(4) Ссылки на смежные задачи (по другому функционалу, по смежным подсистемам и т.д.)  
#### Первичные исходные данные по задаче:  
(1) Документация и описания, необходимые для понимания задачи  
(2) МетаДанные  
#### Требования:  
(1) Обозначить необходимые и достаточные  требования:  
>* к результату и функционалу  
>* к решению  
>* к составу работ  
>* к срокам исполнения  
(2) Обозначить риски и неопределенности (неполнота исходных данных, возможные изменения исходных данных, требований, сроков, решения, бюджета, состава работ) 
(3) Обозначить приоритеты в оптимизации задачи (соблюдение требований, соблюдение сроков, соблюдение бюджета, риски)  
#### Бюджет задачи:  
>(1) Начальный  
>(2) Плановый  
>(3) Реальный  

### 3. Приоритеты поставленных задач  
#### Приоритеты оптимизации качества разработки (Q=качественно, T=быстро, G=дешево, R=риски)  
>!!!! = !!!!качество (отлично, без вариантов)  
>!!!? = !!!качество, ? (хорошо+выбор QTGRx1)  
>!!?? = !!качество, ?? (средне+выбор QTGRх2)  
>!??? = !качество, ??? (плохо+выбор QTGRх3)  
>???? = качество, ???? (неуд+выбор QTGRх4)  

### 4. Этапы разработки и поддержки в деревьях GIT (GIT branches)  
#### Правила присвоения имен ветвям:  
>username.pack.version.stage.priority  
#### (1) Подпись (nickname, username) разработчика   
#### (2) Обозначение ветви для разделения по функционалу (pack)  
>**0000** Основной функционал (основные функции системы)  
>**000X** Базовый функционал (базовый набор функций и подсистем), уровень X=[1-9]  
>**00Y0** Важный функционал (набор подсистем), уровень Y=[1-9]  
>**0Z00** Дополнительный функционал (набор подсистем), уровень Z=[1-9]  
>**CZYX** Комплексный функционал, уровень C=[1-9]  
### (3) Обозначение номера версии [семантической нумерации версий](https://semver.org/lang/ru/)  
##### .V.AA.BB.CC[.DD] = Номера версий в формате .V.МАЖОРНАЯ.МИНОРНАЯ.ПАТЧ  
Cледует увеличивать:  
##### .AA.BB :  
>МАЖОРНУЮ версию "AA", когда сделаны изменения, "обратно несовместимые" с предыдущими версиями.  
>МИНОРНУЮ "BB" версию, когда добавлена новая функциональность, с сохранением "обратной совместимости".  
##### .CC :  
>ПАТЧ-версию, когда делаются "обратно совместимые" исправления.
##### .DD :  
>Дополнительные обозначения могут использоваться как дополнения к V.МАЖОРНАЯ.МИНОРНАЯ.ПАТЧ формату. Используются для создания предрелизных (тестовых и ожидающих одобрения) версий и обозначения  вариантов исполнения (билд-метаданных).  
[Регулярные выражения](https://regex101.com/) для корректных номеров версий с дополнительными обозначениями:  
`.DD = [.][0-9a-zA-Z]{1,4}`  
`.V.AA.BB.CC[.DD] = [.][Vv][0-9]{1,4}[.][0-9]{1,4}[.][0-9]{1,4}[.][0-9a-zA-Z]{1,4}`  
#### (4) Обозначение этапа в имени ветви
>Аналогично метке задачи:
> 0REQ, 1PRE, 2DOC, 2DEV, 3RED, 3TST, 3RUN, 4SUP, 4INF, 4BUG, 4RAT
>**OK** = стабильная версия (по умолчанию)  

### 5. Сохранение черновиков и промежуточных версий файлов, частота коммитов в общий серверный репозитарий  
#### (1) Новая ветвь (branch)  
>При постановке команде новой задачи (issue)  
>При отправке файлов на редактирование другому исполнителю или другой команде  
>Либо по мере необходимости  
#### (2) Совместная работа над файлами  
>Черновой вариант: при сохранении в общий репозитарий: не чаще 4 раз в сутки (утро, полдень, вечер, ночь)  
>Оптимальный вариант: 2-3 раза в неделю (понедельник&четверг | пн&ср&пт)  
#### (3) Объединение ветвей  
>По необходимости и готовности к объединению  
#### (4) Завершение этапов, задач, сохранение ветвей и истории изменений  
По окончанию сроков исполнения & готовности задач:    
> сохранять финальные версии файлов в стабильной ветви "OK"  
> ??? сохранять альтернативные версии файлов с пометкой "JinC" (Just in Case)  
> ??? сохранять ветви с еженедельной историей изменений с пометкой "WeekStory"   

### 6. Ориентировочный недельный график  
>Подведение итогов недели и корректировка планов: еженедельно, вт  
>День ЗОЖ, спорта, укрепление команды.: чт  
>Вечер неЗОЖ (коммиссии, праздники, гости и т.п.).: пт  
