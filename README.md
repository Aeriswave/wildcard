# Описание формата разработки и поддержки решений  
Назначение: рекомендуется использовать для подготовки к проекту, проектной работе, разработке решений и проектной документации, внедрения, эксплуатации  

## 0. Ориентировочный недельный график  
>Подведение итогов недели и корректировка планов: еженедельно, вт  
>День ЗОЖ, спорта, укрепление команды.: чт  
>Вечер неЗОЖ (коммиссии, праздники, гости и т.п.).: пт  

## 1. Проектная работа
### 1.1. Проект  
Цели проекта  
Задачи проекта  
Применение проекта  
Жизненный цикл проекта  
Группа проектов  

### 1.2. Задачи (issue)  
Определение  
Автор  
Ответственный (Assignees)  
Описание
Исходные данные
Требования к результату
Приоритеты
Этапы и метки задачи (Labels)  
История задачи  
Результат выполнения задачи  

### 1.3. Вехи (Milestones) 

## 2. Жизненный цикл 
### 2.1. Проекты 
#### (1) Подготовка  
#### (2) Разработка  
#### (3) Сопровождение (поддержка) проекта  
##### 4ASK, 4BUG, 4RAT, 4SUP  
> Режимы приема заявок (задач)  
> Категории заявок (задач)  
> Режимы отработки заявок (задач)    
#### (4) Развитие проекта  
#### (5) Завершение  

### 2.2. Задачи  
##### Правила присвоения имен задачам:  
Коротко обозначить: подсистему, функционал и цель создания задачи  
##### Правила создания первичного описания задачи:  
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
#### Требования к результату выполнения задачи:  
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

#### Этапы и метки задачи (Labels)  
#### История задачи  
#### Результат выполнения задачи   

## 3. Решения
**Решение** (solution) - это инструментарий для достижения заявленных целей и решения поставленных задач, состоящий из модулей с определенным набором функционала  
### 3.1. Состав решения
**Экосистема решения** (eco) - включает в себя необходимые и достаточные на всех этапах жизненного цикла для разработки, использования, обслуживания и утилизации решения:  
- ***документацию***  
- ***инструментарий***  
- ***ресурсы и финансирование***  

**Модули** (module) - компоненты решения (другие решения, входящие в его состав в качестве модулей)  
**Комплекс решений** (complex) - комплексный инструментарий, состоящий из нескольких решений  
**Набор функционала** (pack) - функционал, предоставляемый решением или модулем  
**Уровень функционала** (level) - сгруппированный по определенным признакам функционал решения или модуля  
**Версия** (version) - один из разработанных вариантов решения или модуля  
**Репозитарий** (repositary) - история изменений версий решения, представленная в файлах, размещенных в папке репозитария и сгруппированных по версиям репозитария.  
**Хранилище репозитария** - место хранения копии репозитария (локальное или общее на сервере)  

### 3.2. Жизненный цикл решения
#### (1) Подготовка к разработке  
#### (2) Разработка    
#### (3) Сопровождение    
#### (4) Продажи    
#### (5) Развитие  
#### (6) Завершение развития    
#### (7) Завершение продаж  
#### (8) Завершение сопровождения  
#### (9) Завершение финансирования  

### 3.3. Репозитарий решения   
#### Термины  
**Каталог (папка) репозитария** - папка (каталог) решения, где размещены файлы и папки репозитария.  
**Конфигурация репозитария** - хранится в служебных файлах и папках репозитария репозитария.  
>**Файлы** - указатель на набор данных, сохраненных в файловой системе под одним именем.  
>**Папки** или **Каталоги** - указатель на набор файлов, сохраненных в файловой системе под одним именем.  
**НЕИндексируемые файлы** - это файлы репозитария, для которых в репозитарии не применяется контроль версий (т.е. для всех версиях репозитария существует только одна версия такого файла).  
> В GIT Список таких файлов задается в файле ".gitignore"  
**Индексируемые файлы** - это файлов репозитария, для которых в репозитарии применяется контроль версий (т.е. для разных версий репозитария могут существовать более одной версии такого файла).  
**Снимок репозитария** (snapshot) или **Версия** - вариант сохраненных в репозитарии файлов, относящихся к одной версия репозитария.  
**Указатель на снимок** - это ссылка на снимок одной из версий репозитария.  
**Ветвь** (Branch) - это название цепочки указателей на последовательные снимки репозитария, сохраненные в соответствие с порядком их создания.  
**Указатель на ветвь** - это указатель на самый свежий снимок в ветви. При сохранении изменений в ветви репозитария сохраняется указатель на новый снимок репозитария.  
**Дерево** (TREE) - это список ветвей репозитария.  
**Метка** (TAG) - именованный указатель на версию репозитария (аналогично ветви, но без обновления указателей на новые версии репозитария)   
**Авторская метка** (aTAG) - это метка с указанием автора, его электронной почты, даты и комментария  
**Подписанная авторская метка** (sTAG) - это авторская метка, подтвержденная "секретным кодом" автора (GPG)  

#### Действия с локальным репозитарием  
**Инициализация** (init) инициализация репозитария в каталоге.  
**Добавление** (add) файлов и папок репозитарии в список индексируемых репозитарием.  
**Игнорирование** репозитарием файлов (создание списка игнорируемых репозитарием файлов (.gitignore)).  
**Сохранение изменений** (commit) в репозитарии - это создание нового снимка репозитария и добавление его к ветви репозитария.  
**Извлечение файла** (checkout) из репозитария - это получение последней версии файла из ветви репозитария.  
**Объединение ветвей** (merge) репозитария -  объединение в единое целое файлов из снимков, относящихся к разным ветвям репозитария.  

#### Действия с репозитарием хранилища  
**Клонирование** (clone) репозитария на компьютер пользователя - это копирование репозитария из хранилища.  
**Синхронизация** (fetch) локального репозитария с репозитарием хранилища - это получение локальным репозитарием данных репозитария из хранилища.  
**Получение** (pull) репозитария на компьютер пользователя - это получение данных репозитария из ветви в хранилище и объединение их ветвью локальном репозитарии.  
**Отправка** (push) локального репозитария в хранилище - это отправка последней версии снимка из ветви репозитария в хранилище.  
**Запрос на добавление изменений** (pull request) -  запрос на добавление нового снимка в ветвь репозитария.  
**Запрос на объединение ветвей** (merge request) -  запрос на объединение файлов из снимков, относящихся к разным ветвям репозитария.  

#### Каталоги (папки) решения  
>**./** Корневая папка (каталог) решения  
>**./BOOK** Для проектной и эксплутационной документации, книг, описаний  
>**./TOOL** Инструментарий  
>**./GOLD** Условия и результат оплаты  
>**./WARE** Решение  

#### Функционал решения или модуля (pack)  
>**0000** Основной функционал (основные функции системы)  
>**000X** Базовый функционал (базовый набор функций и подсистем), уровень X=[1-9]  
>**00Y0** Важный функционал (набор подсистем), уровень Y=[1-9]  
>**0Z00** Дополнительный функционал (набор подсистем), уровень Z=[1-9]  
>**CZYX** Комплексный функционал, уровень C=[1-9]  

### 3.4. Ветви (branch), версии (version), этапы (stage) и метки (tag)  
#### Правила присвоения имен ветвям и меткам:  
(1) Подпись (sign) разработчика  
(2) Название решения (solution)  
(3) Название модуля (module)  
(4) Расширенное обозначение функционала (pack) решения или модуля
Примеры назначения имен ветвям и меткам:  
>sign.solution.version.stage.priority (для основного функционала решения)  
>sign.solution.pack.version.stage.priority  
>sign.module.version.stage.priority (для основного функционала модуля)  
>sign.module.pack.version.stage.priority  

#### Обозначение номера версии решений и модулей
На основе [семантической нумерации версий](https://semver.org/lang/ru/)  
>solution.pack.version  
>module.pack.version  
>.V.AA.BB.CC[.DD] = Номера версий в формате .V.МАЖОРНАЯ.МИНОРНАЯ.ПАТЧ  

Cледует увеличивать:  
>.AA.BB :  
МАЖОРНУЮ версию "AA", когда сделаны изменения, "обратно несовместимые" с предыдущими версиями.  
МИНОРНУЮ "BB" версию, когда добавлена новая функциональность, с сохранением "обратной совместимости".  
>.CC :  
ПАТЧ-версию, когда делаются "обратно совместимые" исправления.
>.DD :  
Дополнительные обозначения могут использоваться как дополнения к V.МАЖОРНАЯ.МИНОРНАЯ.ПАТЧ формату. Используются для создания предрелизных (тестовых и ожидающих одобрения) версий и обозначения  вариантов исполнения (билд-метаданных).  
[Регулярные выражения](https://regex101.com/) для корректных номеров версий с дополнительными обозначениями:  
`.DD = [.][0-9a-zA-Z]{1,4}`  
`.V.AA.BB.CC[.DD] = [.][Vv][0-9]{1,4}[.][0-9]{1,4}[.][0-9]{1,4}[.][0-9a-zA-Z]{1,4}`  

#### Этапы жизненного цикла решения (stage) в обозначениях версий решений и модулей     
Выполняется аналогично присвоенной метки задачи:  
> 0INF, 0REQ, 1PRE, 2DOC, 2DEV, 3RED, 3TST, 3END, 3RUN, 4ASK, 4BUG, 4RAT, 4SUP  
>**OK** = проверенная версия (по умолчанию)  

### 3.5. Сохранение черновиков и промежуточных версий файлов, частота коммитов в общий серверный репозитарий  
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
