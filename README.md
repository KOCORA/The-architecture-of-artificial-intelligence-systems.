# **Лабораторные работы**

*****************************************

# Лабораторная работа 1: Определение границ проекта

В мире бизнеса, где компании приходится сталкиваться с многочисленными конкурентами, затраты на привлечение новых клиентов очень высоки. Поэтому для компаний более важным является удержание существующих клиентов. Поэтому компания должна лучше понимать поведение своих клиентов, чтобы удержать их. Один из способов сделать это - создать модель машинного обучения или искусственной нейронной сети, которая может предсказать, какие клиенты, скорее всего, перейдут на другое обслуживание. Это позволит компании лучше ориентироваться и удерживать клиентов, которые подвержены высокому риску оттока.

В этом проекте мы изучим набор данных телекоммуникационной компании и создадим модель для предсказания того, какие клиенты с наибольшей вероятностью перейдут в другую компанию. Мы будем использовать различные алгоритмы машинного обучения, чтобы сравнить их эффективность и выбрать лучшую модель.

Ограничения` любого проекта машинного обучения зависят от нескольких факторов, таких как качество данных, сложность модели, используемые алгоритмы и доступные ресурсы. Когда речь идет о прогнозировании расторжения контракта с клиентом с помощью машинного обучения, ограничения могут быть следующими:

>>1. Качество данных: Качество данных является ключевым фактором при использовании любого набора данных для машинного обучения. Данные могут быть неполными, неточными или необъективными, что может повлиять на точность моделей машинного обучения.

>>2. Сложность модели: чем сложнее модель машинного обучения, тем труднее ее понять и интерпретировать. Кроме того, слишком сложные модели могут привести к переобучению и снижению производительности на неизвестных данных.

>>3. Используемые алгоритмы: Выбор алгоритмов машинного обучения зависит от характеристик данных и целей проекта. Важно выбрать подходящий алгоритм для данных и оптимизировать его производительность.

>>4. Доступные ресурсы: Проекты машинного обучения могут потребовать значительных ресурсов, таких как мощные компьютеры или большие ресурсы для хранения данных. Таким образом, ограниченность ресурсов может повлиять на возможность запуска алгоритмов или обработки больших объемов данных.

Таким образом, ограничения любого проекта машинного обучения на наборе данных Telco Customer Churn могут включать качество данных, сложность модели, используемые алгоритмы и доступные ресурсы. Важно учитывать эти факторы, чтобы максимально повысить точность и производительность моделей машинного обучения.

## Выбор предметной области

Выбор тематики очень важен в проекте машинного обучения, так как он определяет данные, которые необходимо собирать, и методы, которые будут использоваться для анализа этих данных. Необходимо выбирать проблематику, которая имеет практический или научный интерес и обладает набором данных, подходящим для анализа.

В рамках проекта на основе набора данных Telco Customer Churn была выбрана проблематика прогнозирования расторжения договора клиентами телекоммуникационной компании. Это актуальная тематика, так как удержание клиентов является важным аспектом для компаний, которые стремятся удержать своих клиентов, чтобы сохранить свой объем продаж. Набор данных "Telco Customer Churn" подходит для данной проблематики, так как он содержит информацию о характеристиках клиентов и их решении о расторжении или продлении договора.

## Обзор существующих решений

Существует несколько решений для прогнозирования расторжения договора с клиентом. Наиболее часто используемыми методами машинного обучения являются:

>>Логистическая регрессия: этот метод предполагает построение регрессионной модели для прогнозирования вероятности расторжения контракта. Она относительно проста в применении и может дать точные результаты, если характеристики клиента подобраны правильно.

>>Деревья решений: этот метод предполагает построение дерева решений для прогнозирования того, расторгнет ли клиент свой контракт или нет. Деревья решений просты для понимания и интерпретации, но могут быть менее точными, чем другие методы машинного обучения.

>>Нейронные сети: этот метод предполагает построение нейросетевой модели для прогнозирования вероятности расторжения контракта. Нейронные сети могут быть очень точными, но могут быть более сложными для реализации и интерпретации, чем другие методы машинного обучения.

>>Методы классификации: этот метод предполагает использование алгоритмов классификации, таких как наивная классификация Байеса или k-nearest neighbour, для прогнозирования того, расторгнет ли клиент свой контракт или нет. Эти методы могут быть простыми в реализации и интерпретации, но могут быть менее точными, чем другие методы машинного обучения.

Следует отметить, что каждый из этих методов имеет свои преимущества и недостатки в зависимости от характера данных и целей проекта. Поэтому важно выбрать подходящую методику в зависимости от характеристик набора данных и требований к прогнозированию. Кроме того, может быть полезно использовать методы обработки данных, такие как уменьшение размерности, для улучшения качества прогнозирования.

## Выбор датасета

Мы будем использовать набор данных "Telco Customer Churn" с сайта Kaggle: 

Dataset: Telco costumer churn (Kaggle) URL : [Здесь](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

Автор : Blastchar.

Лицензия: Data files © Original Authors.

Ссылка на созданный репозиторий: https://github.com/KOCORA/The-architecture-of-artificial-intelligence-systems.

Набор данных "Telco Customer Churn" содержит информацию о клиентах телекоммуникационной компании и истории расторжения их контрактов. Набор данных состоит из 7043 записей и 21 переменной. Ниже приводится краткое описание переменных:

+ **CustomerID**: Уникальный идентификатор каждого клиента в базе данных.
+ **Gender**: Пол клиента (мужской или женский).
+ **SeniorCitizen**: указывает, является ли клиент пенсионером или нет.
+ **Partner: указывает**, есть ли у клиента партнер или нет.
+ **Dependents: указывает**, есть ли у клиента иждивенцы или нет.
+ **Tenure**: Количество месяцев, в течение которых клиент является абонентом телекоммуникационной компании.
+ **PhoneService**: указывает на наличие или отсутствие у клиента телефонной связи.
+ **MultipleLines**: указывает, есть ли у клиента несколько телефонных линий.
+ **InternetService**: указывает тип интернет-услуг, которыми пользуется клиент (DSL, оптоволокно, отсутствие услуг).
+ **OnlineSecurity**: указывает, есть ли у клиента услуга онлайн-безопасности.
+ **OnlineBackup**: указывает, есть ли у клиента услуга резервного копирования.
+ **DeviceProtection**: указывает, есть ли у клиента услуга защиты устройства.
+ **TechSupport**: указывает, есть ли у клиента служба технической поддержки или нет.
+ **StreamingTV**: указывает, есть ли у клиента услуга потокового телевидения или нет.
+ **StreamingMovies**: указывает, есть ли у клиента услуга потокового просмотра фильмов или нет.
+ **Contract**: указывает тип контракта, который клиент заключил с телекоммуникационной компанией (ежемесячный, годовой, на два года).
+ **PaperlessBilling**: указывает, использует ли клиент безбумажный биллинг или нет.
+ **PaymentMethod**: указывает способ оплаты, который использует клиент (банковский перевод, кредитная карта, электронный чек, автоматический платеж).
+ **MonthlyCharges**: ежемесячная сумма, которую клиент должен заплатить за телекоммуникационные услуги.
+ **TotalCharges**: общая сумма, которую клиент заплатил за телекоммуникационные услуги с момента регистрации.
+ **Churn: указывает**, отписался ли клиент от телекоммуникационной компании.

## Цели и задачи

### Цель: 

разработать модель машинного обучения, способную предсказывать прекращение обслуживания клиентов телекоммуникационной компании, используя набор данных Telco Customer Churn.

### Задачи :

Для реализации этого проекта мы выполним следующие задачи:

+ Анализ существующих решений;
+ Сбор и подготовка данных: сбор соответствующих данных из набора данных Telco Customer Churn, очистка данных и подготовка их к анализу.
+ Разведочный анализ данных: проведение статистического анализа данных для выявления тенденций и взаимосвязей между различными переменными.
+ Выбор признаков: выбор наиболее важных признаков для прогнозирования оттока клиентов.
+ Построение и обучение моделей: создание различных моделей машинного обучения с использованием таких алгоритмов, как логистическая регрессия, многослойный перцептрон, случайный лес и машина опорных векторов (SVM), и обучение этих моделей на обученных данных.
+ Оценка модели: оценка эффективности каждой модели с помощью таких показателей, как точность, прецизионность, отзыв и F1 score.
+ Оптимизация модели: корректировка гиперпараметров модели для улучшения ее производительности.
+ Сравнение моделей: сравнение производительности трех или четырех моделей, чтобы определить, какая из них наиболее эффективна в прогнозировании расторжения договора с клиентом.
+ Развертывание модели: развертывание выбранной модели для использования в режиме реального времени.

![](https://github.com/KOCORA/The-architecture-of-artificial-intelligence-systems./blob/master/Image10.png)

Рисунок 1: распределение переменной TotalCharges в зависимости от расторжения договора клиента в наборе данных Telco Customer Churn.

Эта гистограмма показывает распределение значений переменной "TotalCharges" в наборе данных "Telco Customer Churn". Горизонтальная ось представляет значения "TotalCharges", а вертикальная ось - количество вхождений каждого значения. Столбцы гистограммы складываются для каждого значения переменной "Churn" (Yes или No). Это позволяет визуализировать распределение значений "TotalCharges" для клиентов, которые расторгли контракт (Churn = 1) и для тех, кто этого не сделал (Churn = 0). Можно увидеть, есть ли существенная разница в распределении этой переменной между двумя группами клиентов.


## Инициализация проекта

Данные загрузить на гитхаб : https://github.com/KOCORA/The-architecture-of-artificial-intelligence-systems./blob/master/WA_Fn-UseC_-Telco-Customer-Churn.csv. 

# Лабораторная работа 2: Разработка архитектуры системы

Для того чтобы реализовать различные диаграммы UML (компонентные, коммуникационные и деятельностные) на наборе данных "Telco Customer Churn", мы должны сначала проанализировать отношения между различными компонентами системы.  Представленные различные диаграммы UML могут быть очень полезны для моделирования и понимания различных аспектов системы "Telco Customer Churn".

![На рисунке 1 показана диаграмма компонентов, описывающая структуру нашей системы.](https://github.com/KOCORA/The-architecture-of-artificial-intelligence-systems./blob/master/Component%20diagram.png).
Рис 1. Описание архитектуры нашей системы в виде диаграммы компонентов UML.

Эта диаграмма может быть использована для понимания общей структуры системы и взаимосвязей между различными компонентами. Она может помочь прояснить, как различные компоненты взаимодействуют для создания полной системы, способной анализировать данные о расторжении договоров с клиентами для данного набора данных.

![На рисунке 2 показана диаграмма связи нашей системы.](https://github.com/KOCORA/The-architecture-of-artificial-intelligence-systems./blob/master/Communication%20diagram.png).
Рис 2. Описание архитектуры нашей системы в виде диаграммы связей UML.

Эта диаграмма может быть использована для понимания взаимодействия между различными субъектами, участвующими в обработке данных о расторжении договоров с клиентами для этого набора данных. Она может помочь прояснить, как различные участники взаимодействуют для создания комплексной системы, способной анализировать данные о расторжении договоров с клиентами и представлять результаты анализа конечным пользователям.

![На рисунке 3 показана диаграмма деятельности нашей системы.]https://github.com/KOCORA/The-architecture-of-artificial-intelligence-systems./blob/master/Activity%20diagram.png).
Рис 3. Диаграмма деятельности процесса работы системы.

Эта диаграмма деятельности может быть использована для понимания процесса обработки данных об оттоке клиентов с помощью компьютерной системы. Она поможет визуализировать этапы процесса и определить действия, необходимые для построения прогнозной модели для клиентов, подверженных риску оттока.

# Лабораторная работа 3: Подготовка исходных данных

Мы выполнили эту задачу в google colab, а затем сохранили в нашем Github. В приложении ссылка на наш код для предварительной обработки набора данных:
https://github.com/KOCORA/The-architecture-of-artificial-intelligence systems./blob/master/Costumer_churn.ipynb 
