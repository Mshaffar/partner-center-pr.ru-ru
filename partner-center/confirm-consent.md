---
title: Подтверждение принятия клиентом условий Клиентского соглашения Майкрософт
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Узнайте, как подтвердить принятие клиентом условий Клиентского соглашения Майкрософт. Это может потребоваться для заказа продуктов и услуг Майкрософт для клиентов.
author: LauraBrenner
ms.author: labrenne
keywords: Клиент, клиенты, согласие, MCA, Клиентское соглашение Майкрософт, шаблоны клиентских соглашений
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d45f04c8ee1a8d8715f5c6484598ecaca83b1f1
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908151"
---
# <a name="overview-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Обзор: Подтверждение принятия клиентом условий Клиентского соглашения Майкрософт

**Относится к**
-  Центр партнеров

**Соответствующие роли**

- Агент по администрированию
- Агент по продажам

> [!NOTE]
> В настоящее время ресурс соглашения поддерживается только Центром партнеров в общедоступном облаке Майкрософт. Это не относится к следующим службам:
> * Центр партнеров, предоставляемый 21Vianet
> * Центр партнеров Microsoft Cloud в Германии
> * Центр партнеров для Microsoft Cloud for US Government

>[!NOTE]
>С 31 января 2020 года все клиенты, существующие и новые, должны подписать новое Клиентское соглашение Майкрософт. Чтобы узнать больше, прочитайте о [подтверждении принятия клиентом условий клиентского договора с Майкрософт](confirm-customer-agreement.md).

Как партнеру, вам необходимо получить от клиента принятие им условий клиентского соглашения Майкрософт, прежде чем вы сможете заказывать продукты и службы корпорации Майкрософт для этого клиента. Чтобы помочь партнерам эффективнее обеспечивать соответствие нормативным требованиям, корпорация Майкрософт просит своих партнеров подтверждать принятие условий соглашения клиентом путем предоставления следующих сведений о клиенте, принявшем условия соглашения.

- Имя

- Фамилия

- Адрес электронной почты

- Номер телефона (необязательно)

- Дата принятия условий

Партнеры с прямым выставлением счетов и косвенные поставщики должны подтвердить принятие клиентом условий Клиентского соглашения Майкрософт при взаимодействии с Центром партнеров или API Центра партнеров. Подтверждение является *обязательным*.

При отсутствии подтверждения для конкретного клиента вступают в силу следующие ограничения.

-    Вы не сможете создавать новые заказы для этого клиента.

-    Вы не сможете изменять количество рабочих мест для имеющихся подписок по местам для этого клиента.

Подтвердить принятие клиентом условий соглашения можно с помощью Центра партнеров или API Центра партнеров. Как это сделать это с помощью API Центра партнеров описывается в следующих разделах: 

-   [Получение подтверждения согласия клиента](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Получение метаданных соглашения](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Подтверждение согласия клиента](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Это относится как к рабочим средам, так и к песочницам.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Подтверждение принятия клиентом условий соглашения в Центре партнеров

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Подтверждение принятия условий соглашения новым клиентом

Используйте следующую процедуру для подтверждения принятия клиентом условий соглашения при создании нового арендатора клиента в Центре партнеров. Обратите внимание на то, что для выполнения этой процедуры вы должны быть агентом администрирования или агентом по продажам.

1. Выберите **Клиенты**, затем — **Новый клиент**, после чего выберите **Сведения об учетной записи**.
2. Введите соответствующие сведения в полях **Компания** и **Основное контактное лицо**.

![Сведения о компании](images/mca/mca1.png)

3. В разделе **Клиентское соглашение Майкрософт** установите флажок **The customer has accepted the latest Microsoft customer agreement** (Клиент принял условия последнего Клиентского соглашения Майкрософт).
4. В разделе **Дата принятия условий соглашения** введите соответствующую дату. Здесь нельзя указать дату, которая еще не наступила.
5. Введите данные о пользователе, который сообщил о принятии им условий соглашения.

![Добавление даты принятия условий](images/mca/MCA3.png)

По умолчанию отображаются основные контактные сведения пользователя. Если они неправильные, выберите **Обновить**, а затем введите **Имя**, **Фамилию**, **Адрес электронной почты** и **Номер телефона* (необязательно) пользователя, который принял условия соглашения.

6. Выберите **Далее**, чтобы продолжить выполнение оставшихся действий по созданию клиента.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Подтверждение принятия условий соглашения существующим клиентом

Для выполнения этой процедуры вы должны быть агентом администрирования или агентом по продажам.

1. Выберите **Клиенты**, а затем найдите и выберите необходимого клиента.
2. Выберите **Сведения об учетной записи**.
3. В разделе **Клиентское соглашение Майкрософт** выберите **Обновить**.

![Обновление:](images/mca/mca4.png)

4. Введите **Имя**, **Фамилию**, **Адрес электронной почты** и **Номер телефона** (необязательно) пользователя, принявшего условия соглашения.
5. В разделе **Дата принятия условий соглашения** введите соответствующую дату. Здесь нельзя указать дату, которая еще не наступила.
6. Выберите **Сохранить и продолжить**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Подтверждение принятия клиентом условий соглашения при создании нового заказа для существующего клиента

Если вы пытаетесь создать новый заказ для существующего клиента, от которого еще не получено подтверждение принятия условий соглашения, вам будет предложено выполнить процедуру подтверждения. Выполните следующие действия.

1. Введите **Имя**, **Фамилию**, **Адрес электронной почты** и **Номер телефона** (необязательно) пользователя, принявшего условия соглашения.
2. В разделе **Дата принятия условий соглашения** введите соответствующую дату. Здесь нельзя указать дату, которая еще не наступила.
3. Выберите **Сохранить и продолжить**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Получение подтверждения о принятии условий соглашения существующим клиентом

Вы можете получить подтверждение о принятии условий соглашения существующим клиентом, которое вы предоставляли ранее, используя описанную ниже процедуру. Для выполнения этой процедуры вы должны быть агентом администрирования или агентом по продажам.

1. Выберите **Клиенты**, а затем найдите и выберите необходимого клиента.
2. Выберите **Сведения об учетной записи**.
3. В разделе **Клиентское соглашение Майкрософт** вы увидите, было ли предоставлено подтверждение для этого клиента.
