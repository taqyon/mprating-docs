---
cssclass: wide
alias: оплата
---

*Последнее редактирование: <%+ tp.file.last_modified_date() %>*

# Payment

Оплата. 

## Способы оплаты

Для оплаты заявок доступно два способа оплаты: 

- СБП, QR Код
- Сервис оплаты 

### СБП, QR Код

Оплата с помощью [системы быстрых платежей, через QR код.](https://sbp.nspk.ru/business/) 

При этом методе оплаты, сервис должен брать QR код с сайта [[MarketPlace|маркетплейса]] и отображать его в собственном интерфейсе. В таком случае [[Client|клиент]] сможет оплатить выкуп «на месте и сразу». 

#### Что означает «Сервис должен брать QR код с сайта маркетплейса»?

Это означает, что при выполнении [[3. Processing of the Order| заявки]], [[MarketPlaceAccount|учетная запись]] выбирает в качестве способа оплаты СБП QR код. И при инициализации этого метода оплаты на [[MarketPlace|маркетплейсе]], маркетплейс формирует изображение QR кода в своём окружении. Это изображение мы должны отобразить у себя в интерфейсе для [[Client|клиента]].

### Сервис оплаты

>[!tip] Обратите внимание!
>
> Что такой метод оплаты, доступен **только** для режима работы выкупа — [[BuyBack#Органичный выкуп| органичный выкуп.]]


Предполагается что при таком методе оплаты, [[Client|клиент]] подключает свою банковскую карту. И по мере выполнения [[Task | выкупов]], сервис списывает средства с этой карты. 