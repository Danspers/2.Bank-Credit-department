﻿# Описание проекта

Заказчик — кредитный отдел банка. Нужно разобраться, влияет ли семейное положение и количество детей клиента на _факт погашения кредита_ в срок. Входные данные от банка — статистика о платёжеспособности клиентов.

Результаты исследования будут учтены при построении _модели кредитного скоринга_ — специальной системы, которая оценивает способность потенциального заёмщика вернуть кредит банку.

**План работы:**
1. Обзор данных,
2. Предобработка данных,
3. Исследование данных,
4. Итоги исследования.

## Общий вывод.

В ходе исследования получилось проверить предположения о наличии зависимости между параметрами заёмщика и вероятностью возврата кредита в срок, и оценить на сколько эти параметры влияют на вероятность. Кратко:
- **Дети:** их отсутствие положительно сказывается на вероятности.
- **Семейный статус:** заёмщики, не бывавшие в браке, или, не зарегистрировавшие его, имеют наибольший риск не возврата кредита. Средний риск соответствует женатым клиентам, или находящимся замужем. Минимальный риск у группы людей, уже побывавших в браке.
- **Уровень дохода:** заёмщики группы D (доход ниже среднего) чаще возвращают кредиты в срок в сравнение с группой С (средний доход). Ещё реже возвращают кредит заёмщики из групп A и E, но этот вывод может оказаться недостоверным из-за их малой численности. Тоже самое касается группы B, которая показала минимальный риск не возврата кредита.

![График зависимости доли невозвращенных займов от уровня дохода](https://github.com/danspers/2.Bank-Credit-department/raw/main/total_income_category.jpg)

- **Цель:** Кредиты предназначенные для *проведения свадеб* и совершению *операций с недвижимостью* имеют наименьший риск.

На основе полученных зависимостей можно комплексно применять эти параметры для прогнозирования вероятности возврата кредита в срок для потенциального клиента.