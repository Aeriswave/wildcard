## Шаблон папки репозитария:
Назначение: подготовка к проекту (пресейл), проектная работа, разработка решений и проектной документации, внедрение, эксплуатация
### 1. Папки репозитария:
>**./BOOK** Для проектной и эксплутационной документации, книг, описаний  
>**./TOOL** Разработанный инструментарий  
>**./GOLD** Условия и результат оплаты  

### 2. Шаблон нового репозитария с набором ветвлений (branches)
#### (1) Основные ветви (branches) для разделения на этапы разработки и использования:
>**1PRE** = подготовка к разработке, сбор исходных данных, систематизация, анализ, формирование требований и подготовительной документации  
>**2DEV** = версия в разработке, создание прототипа  
>**2TST** = тестирование прототипа  
>**BugFIX** = исправление багов  
>**PATCH** = временное решение проблемы (Патч, заплатка)  
>**RUN** = тестовая эксплуатации (перед сдачей результата)  
>**SUP** = разработано, проверено, согласовано, осуществляется техподдержка  
>**OK** = стабильная версия, без техподдержки (по умолчанию)  

#### (2) Дополнительные ветвления для разделения
>**0000** Базовый функционал (набор подсистем)  
>**000X** Основной функционал (набор подсистем), уровень X={1...9}  
>**00Y0** Важный функционал (набор подсистем), уровень Y={1...9}  
>**0Z00** Дополнительный функционал (набор подсистем), уровень Z={1...9}  
>**CZYX** Комплексный функционал, уровень C={1...9}

### 3. [Семантическая нумерация версий](https://semver.org/lang/ru/) в ветках
##### .V.AA.BB.CC = Номера версий ветвлений в формате .V.МАЖОРНАЯ.МИНОРНАЯ.ПАТЧ
Cледует увеличивать:
##### AA = {0...99999}:
>МАЖОРНУЮ версию, когда сделаны обратно несовместимые изменения API.  
>МИНОРНУЮ версию, когда вы добавляете новую функциональность, не нарушая обратной совместимости.
##### BB = {0...99999}:
>ПАТЧ-версию, когда вы делаете обратно совместимые исправления.
##### CC= {0...99999}:
>Дополнительные обозначения для предрелизных и билд-метаданных возможны как дополнения к V.МАЖОРНАЯ.МИНОРНАЯ.ПАТЧ формату.  

### 4. Оценка поставленных исполнителю задач
#### Приоритеты оптимизации качества разработки (Q=качественно, T=быстро, G=дешево, R=риски)
>!!!! = !!!!качество (отлично, без вариантов)  
>!!!? = !!!качество, ? (хорошо+выбор QTGRx1)  
>!!?? = !!качество, ?? (средне+выбор QTGRх2)  
>!??? = !качество, ??? (плохо+выбор QTGRх3)  
>???? = качество, ???? (неуд+выбор QTGRх4)  
