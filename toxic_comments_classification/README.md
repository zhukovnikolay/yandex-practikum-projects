# Классификация токсичных комментариев 

## Статус проекта
Завершен

## Описание проекта
Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию.
Обучите модель классифицировать комментарии на позитивные и негативные. В вашем распоряжении набор данных с разметкой о токсичности правок.

## Описание данных

- text - содержит текст комментария
- toxic - целевой признак

## Вывод
В ходе выполнения проекта были выполнены следующие задачи:
1. Проанализированы комментарии.
2. Подготовлен класс-обработчик данных, который очищает, токенизирует и лемматизирует данные.
3. Разработаны две базовых модели.
4. Построены модели на TfidfVectorizer и эмбеддингах. Для моделей проведен подбор гиперпараметров.

Лучший результат показала модель бустинга на TfidfVectorizer, она смогла достичь требуего уровня метрики f1 (0.772). Именно ее можно считать основной.

Модели на эмбеддингах (BERT) показали результат хуже, чем у базовых моделей. Возможно, это связано с малым числом объектов для обучения или недостаточной обработкой комментариев.

## Используемые библиотеки
*pandas, numpy, re, nltk, pymorphy2, wordcloud, sklearn, lightgbm, catboost, torch, transformers, matplotlib, seaborn*