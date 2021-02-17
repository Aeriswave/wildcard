# Описание формата разработки и поддержки решений  
Назначение: рекомендуется использовать для подготовки к проекту, проектной работе, разработке решений и проектной документации, внедрения, эксплуатации  

## Термины и определения  

### Проект  
Цели проекта  
Применение проекта  
Жизненный цикл проекта  
Группа проектов  

### Задачи  
Автор  
Ответственный (Assignees)  
Название  
Описание  
Исходные данные  
Финансирование  
Приоритеты  
Этапы и метки задачи (Labels)  
Требования  
История  
Результат  

### Этапы проекта  
Подготовка  
Разработка  
Поддержка  
Завершение  

### Вехи (Milestones)  

## Решения
**Решение** (solution) - инструментарий для достижения заявленных целей и решения поставленных задач, состоящий из модулей с определенным набором функционала  
**Модули** (module) - компоненты решения (другие решения, входящие в его состав в качестве модулей)  
**Комплекс решений** (complex) - комплексный инструментарий, состоящий из нескольких решений  
**Набор функционала** (pack) - функционал, предоставляемый решением или модулем  
**Уровень функционала** (level) - сгруппированный по определенным признакам функционал решения или модуля  
**Версия** (version) - один из разработанных вариантов решения или модуля  
**Репозитарий** (repositary) - история изменений версий решения, представленная в файлах, размещенных в папке репозитария и сгруппированных по версиям репозитария.  
**Хранилище репозитария** - место хранения копии репозитария (локальное или общее на сервере)
**Экосистема решения** (eco) - включает в себя необходимые и достаточные для разработки, использования, поддержки и утилизации решения:  
-***документацию  
-***инструментарий  
-***ресурсы и финансирование  

### Репозитарий решения   
Включает в себя:  
**Файлы** - наборы данных, сохраненных в файловой системе под одним именем.  
**Папка** - наборы файлов, сохраненных в файловой системе под одним именем.  
**Файловую систему репозитария** - список папок и файлов репозитария.  
**Папки репозитария** - папки файловой системы репозитария.  
**Снимок** (snapshot) или **Версия** - одна из сохраненных версий репозитария.  
**Указатель на снимок** - это ссылка на расположение снимка одной из версий репозитария файла.  
**Ветвь** (Branch) - это название цепочки указателей на последовательные снимки репозитария, сохраненные в соответствие с порядком их создания.  
**Указатель на ветвь** - это указатель на самый свежий снимок в ветви. При сохранении изменений в ветви репозитария сохраняется указатель на новый снимок репозитария.  
**Дерево** - это список ветвей репозитария.  
**Метка** (TAG) - именованный указатель на версию репозитария (аналогично ветви, но без обновления указателей на новые версии репозитария)   
**Авторская метка** (aTAG) - это метка с указанием автора, его электронной почты, даты и комментария     
**Подписанная авторская метка** (sTAG) - это авторская метка, подтвержденная "секретным кодом" автора (GPG) 

**Сохранение изменений** (commit) в репозитарии - это создание снимка текущего состояния репозитария и добавление его к ветви репозитария.  
**Получение файлов из хранилища** (checkout) - это копирование последней версии снимка из ветви репозитария.  
**Запрос на добавление изменений** (pull request) -  запрос на создание нового снимка в ветви репозитария.  
**Запрос на объединение** (merge request) -  запрос на объединение файлов из снимков, относящихся к разным ветвям репозитария.  

#### 1. Папки репозитария:  
>**./BOOK** Для проектной и эксплутационной документации, книг, описаний  
>**./TOOL** Инструментарий  
>**./GOLD** Условия и результат оплаты  
>**./WARE** Решение  

### 2. Задачи:  
#### Правила присвоения имен задачам:  
Коротко обозначить: подсистему, функционал и цель создания задачи  

#### Правила создания первичного описания задачи:  
(1) Обозначить цели задачи, поставить соответствующие метки  
>**0INF** = запрос на предоставление информации  
>**0REQ** = запрос на создание, разработку, выполнение работ  
>**1PRE** = подготовка к разработке, сбор исходных данных, систематизация, анализ, формирование требований и подготовительной документации  
>**2DOC** = разработка и правка документации, описаний, схем, книг, моделей...  
>**2DEV** = развитие (разработка), создание прототипа, разработка нового функционала  
>**3RED** = правки, модификации, изменения, оптимизация существующего функционала  
>**3TST** = тестирование прототипа, функционала, изменений, совместимости  
>**3END** = поддержка, разработка или работы приостановлены или отменены  
>**4SUP** = осуществляется техподдержка (фиксация, диагностика и решение проблем в стабильной версии)  
>**4BUG** = исправление неточностей и небольших ошибок  
>**4RAT** = исправление серьезных ошибок и проблем (патч, заплатка)  
>**4ASK** = нужен ответ на вопрос или консультация  
>**5RUN** = тестовая эксплуатации  
>**LOOP** = похожая задача уже существует  
>**OK** = проверенная версия  

(2) Описание планируемого практического применения результата работ  
(3) Ссылки на проект  
(4) Ссылки на смежные задачи (по смежным подсистемам, функционалу и т.д.)  
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
(1) Начальный  
(2) Плановый  
(3) Реальный  

#### Приоритеты задач  
Приоритеты оптимизации качества разработки (Q=качественно, T=быстро, G=дешево, R=риски)  
>!!!! = !!!!качество (отлично, без вариантов)  
>!!!? = !!!качество, ? (хорошо+выбор QTGRx1)  
>!!?? = !!качество, ?? (средне+выбор QTGRх2)  
>!??? = !качество, ??? (плохо+выбор QTGRх3)  
>???? = качество, ???? (неуд+выбор QTGRх4)  

### 4. Техподдержка  
#### 4ASK, 4BUG, 4RAT, 4SUP  
> Режимы приема заявок  
> Категории заявок  
> Режимы отработки заявок    

### 5. Деревья  
#### Правила присвоения имен ветвям:  
>username.solution.version.stage.priority (для основного функционала решения)  
>username.solution.pack.version.stage.priority  
>username.module.version.stage.priority (для основного функционала модуля)  
>username.module.pack.version.stage.priority  
#### (1) Подпись (nickname, username) разработчика  
#### (2) Решения (solution)  
#### (3) Модуль (module)  
#### (4) Расширенное обозначение функционала (pack) решения или модуля  
>**0000** Основной функционал (основные функции системы)  
>**000X** Базовый функционал (базовый набор функций и подсистем), уровень X=[1-9]  
>**00Y0** Важный функционал (набор подсистем), уровень Y=[1-9]  
>**0Z00** Дополнительный функционал (набор подсистем), уровень Z=[1-9]  
>**CZYX** Комплексный функционал, уровень C=[1-9]  
#### (5) Обозначение номера версии решений и модулей на основе [семантической нумерации версий](https://semver.org/lang/ru/)  
>solution.pack.version  
>module.pack.version  
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
#### (5) Обозначение этапа (stage) в имени ветви  
>Аналогично метке задачи:  
> 0INF, 0REQ, 1PRE, 2DOC, 2DEV, 3RED, 3TST, 3END, 3RUN, 4ASK, 4BUG, 4RAT, 4SUP  
>**OK** = проверенная версия (по умолчанию)  

### 6. Сохранение черновиков и промежуточных версий файлов, частота коммитов в общий серверный репозитарий  
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

### 7. Ориентировочный недельный график  
>Подведение итогов недели и корректировка планов: еженедельно, вт  
>День ЗОЖ, спорта, укрепление команды.: чт  
>Вечер неЗОЖ (коммиссии, праздники, гости и т.п.).: пт  

