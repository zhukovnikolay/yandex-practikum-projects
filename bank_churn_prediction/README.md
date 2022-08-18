# Прогнозирование оттока клиентов банка

Источник данных: https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling

## Статус проекта
Завершен

## Описание проекта
Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Мне предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.

## Описание данных
- RowNumber — индекс строки в данных
- CustomerId — уникальный идентификатор клиента
- Surname — фамилия
- CreditScore — кредитный рейтинг
- Geography — страна проживания
- Gender — пол
- Age — возраст
- Tenure — количество недвижимости у клиента
- Balance — баланс на счёте
- NumOfProducts — количество продуктов банка, используемых клиентом
- HasCrCard — наличие кредитной карты
- IsActiveMember — активность клиента
- EstimatedSalary — предполагаемая зарплата
- Exited — Целевой признак, факт ухода клиента

## Вывод

Основной проблемой был дисбаланс классов (20 % для первого класса). 
Мы рассмотрели три варианта работы с дисбалансом классов: 
- oversampling;
- undersampling;
- установку весов классов в качестве гиперпараметра модели.

Для каждого из методов мы оценили метрики F1-score и AUC ROC для валидационной выборки и пришли к выводу, что оптимальной является подход борьбы с дисбалансом с помощью установки весов классов в качестве гиперпараметра модели.

Результатом работы стала модель на базе CatBoostClassifier со следующими метриками:
- Лучшая модель основана на алгоритме CatBoostClassifier
- Лучший показатель F1 метрики: 0.651
- Лучший показатель ROC-AUC: 0.87.

## Используемые библиотеки
*re, pandas, numpy, sklearn, catboost, matplotlib, seaborn*