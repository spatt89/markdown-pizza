# Домашнее задание Skillfactory
## Разметка markdown и Git

**Сценарий заказа на сайте на сайте пиццерии**

**Акторы**: Пользователь, сайт, банк

**Цель**: оплатить заказ на сайте пиццерии

**Основной сценарий** Оплата картой
1. Пользователь нажимает “оформить заказ” и оплатить картой
2. Сайт отправляет информацию с суммой оплаты в банк
3. Банк возвращает сообщение об успешной оплате
4. Сайт сообщает пользователю об успешной оплате
5. Сайт передает информацию с номером заказа в пиццерию

**Альтернативный сценарий:** оплата наличными при получении
1. Пользователь нажимает оплата “оплата при получении”
2. Сайт возвращает сообщение: оплата курьеру наличными или картой
3. Пользователь нажимает “наличными”
4. Сайт возвращает сообщение, что заказ подтвержден
5. Сайт передает информацию в пиццерию
6. Сайт передает информацию курьеру, что оплата “наличными” при получении.

**Исключение1:**
-Не прошла оплата по банку
-Сайт возвращает сообщение на сайте, что оплата не прошла, попробуйте другие способы оплаты

**Исключение2:**
-Пользователь перешел в меню оплата через банк, но в течении 10 минут не совершает оплату
-Сайт выводит сообщение: Продолжить оплату или отменить заказ?
-Если нет действий, сайт выводит сообщение, что заказ отменен в из-за временного ограничения. Пожалуйста создайте новый заказ.

также сделал изменение в первом файле