# Evaluating (A/B-testing) the effectiveness of a new recommendation system
**Цель**:
Нужно оценить эффективность новой RecSys на платформе онлайн-супермаркета

**Данные**:

orders_ab.csv — информация о заказах:

order_id - id заказа

creation_time - время создания заказа

product_ids - id продукта


products_ab.csv — информация о продуктах:

product_id - id продукта

name - имя продукта

price - цена продукта


users_data_ab.csv — информация о пользователях:

user_id - id пользователя

order_id - id заказа

action - действие

time - точное время заказа

date - дата заказа

group - контрольная группа


**Итоги**:


Из предоставленных датасетов были использованы все.

Количество пользователей в первой группе: 515

Во второй группе: 502.

Время начала и окончания теста в обеих группах примерно одинаковая: 2022-08-26 - 2022-09-08.

Это позволило провести тест без уменьшения количества пользователей в какой-либо группе и не исключать пользователей из групп не соответсвующих по времени.


Согласно проведенным исследованиям:

1. Доход с обеих групп примерно одинаковый:
Совокупный доход с пользователей первой группы: 226742.5 руб.;

Совокупный доход с пользователей второй группы: 226610.8 руб.

2. Сумма покупок на каждого пользователя тоже примерно одинаковая.

3. Общее количество купленных продуктов возросло.

4. Тип продуктов в корзине в среднем тоже возросло.

5. Проверили, не было ли никаких акции во время проведения теста, так как люди склонны покупать "больше товаров за те же деньги". Акции не было.

6. Поменялось ли тип покупаемых продуктов во время внедрения новой RecSys? Распределение примерно одинаковое, значительно ничего не поменялось.

**Вывод**: итоги теста довольно сомнительные: суммы заказов в обеих группах остались прежними, но количество заказов выросло. Ухудшения в доходах не замечено. Можно внедрять новую рекомендационную систему, но необходимо следить за ключевыми показателями.
