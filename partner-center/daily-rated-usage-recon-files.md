---
title: Файлы сверки с оценкой использования по дням
ms.topic: article
ms.date: 05/15/2020
description: Узнайте, как читать файлы сверки с ежедневной оценкой использования в центре партнеров.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3536b1b71dd8378e88ac14726adcca7fa0e08530
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795593"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Узнайте, как считать файлы сверки с оценкой использования в центре партнеров

**Относится к**

- Центр партнеров
- Центр партнеров для Microsoft Cloud for US Government

**Соответствующие роли**

- Агент по администрированию
- Администратор выставления счетов
- Агент по продажам
- Агент службы технической поддержки

В этом разделе объясняется, как считывать файлы сверки с ежедневной оценкой использования.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Поля в файлах сверки с ежедневной оценкой использования

| Столбец | Описание |
| ------ | ----------- |
| PartnerId | Идентификатор партнера в формате GUID. |
| PartnerName | Имя партнера. |
| CustomerId | Уникальный идентификатор Майкрософт для клиента в формате GUID. |
| CustomerName | Название организации клиента, указанное в Центре партнеров. *Этот столбец очень важен для согласования счета со сведениями о системе.* |
| CustomerDomainName | Доменное имя клиента. |
| CustomerCountry | Страна, в которой находится клиент. |
| MpnId | Идентификатор MPN партнера CSP. |
| Tier2MpnId | MPN Идентификатор торгового посредника записи для подписки. |
| InvoiceNumber | Номер счета, в котором отображается указанная транзакция. |
| ProductId | Идентификатор продукта. |
| SkuId | Идентификатор для конкретного номера SKU. |
| AvailabilityId | Идентификатор для доступности конкретного SKU. Показывает, доступен ли номер SKU для покупки в указанной стране, валюте, отрасли и т. д. |
| SkuName | Название для определенного номера SKU. |
| ProductName | Имя продукта. |
| PublisherName | Имя издателя. |
| PublisherId | Идентификатор издателя в формате GUID. |
| SubscriptionDescription | Имя предложения службы, приобретенной клиентом, как указано в прейскуранте. (Это идентично поле для **указывает**). |
| SubscriptionId | Уникальный идентификатор подписки платформы выставления счетов Майкрософт. Не используется для сверки. *Этот идентификатор не совпадает с **идентификатором подписки** в консоли администратора партнера.* |
| ChargeStartDate | Дата начала цикла выставления счетов (за исключением даты представления ранее неоплаченных скрытых данных об использовании из предыдущего цикла выставления счетов). Этим временем всегда является начало дня — 0:00. |
| ChargeEndDate | Дата окончания цикла выставления счетов (за исключением даты представления ранее неоплаченных скрытых данных об использовании из предыдущего цикла Билинг). Временем всегда является конец дня, 23:59. |
| UsageDate | Дата использования службы. |
| MeterType | Тип счетчика. |
| MeterCategory | Служба верхнего уровня, которая использовалась. |
| MeterId | Идентификатор используемого счетчика. |
| MeterSubCategory | Тип службы Azure, которая может повлиять на скорость. |
| MeterName | Единица измерения для потребляемого измерения. |
| MeterRegion | Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется. |
| Единицы | Единица **имени**ресурса. |
| ResourceLocation | Центр обработки данных, в котором работает счетчик. |
| ConsumedService | Используемая служба платформы Azure. |
| ResourceGroup | Представляет контейнер, содержащий связанные ресурсы для решения Azure. |
| ResourceURI | URI используемого ресурса. |
| ChargeType | Тип оплаты или коррекции.  |
| UnitPrice | Цена за лицензию, опубликованная в прейскуранте на момент приобретения. Убедитесь, что эта цена соответствует информации, хранящейся в системе выставления счетов во время сверки. |
| Количество | Число лицензий. Убедитесь, что эта цена соответствует информации, хранящейся в системе выставления счетов во время сверки. |
| Единицах UnitType | Тип единицы измерения, за которую наследуется данный счетчик.  |
| биллингпретакстотал | Общая сумма выставления счетов перед налогами. |
| BillingCurrency | Валюта в географическом регионе клиента. |
| приЦингпретакстотал | Цены перед добавлением налогов. |
| PricingCurrency | Валюта в прайс-листе. |
| ServiceInfo1 | Количество подключений служебной шины, которые были подготовлены и использованы в определенный день. |
| ServiceInfo2 | Устаревшее поле, которое фиксирует необязательные метаданные, относящиеся к службе. |
| Теги | Представляет логическую организацию ресурсов Azure, заданную пользователем. |
| AdditionalInfo | Любые дополнительные сведения, не указанные в других столбцах. |
| еффективеунитприце | Фактическое значение, оплачиваемое за единицу, включая скидки, полученные кредиты и т. д. |
| пктобцексчанжерате | Обменный курс, применяемый для валюты цены к валюте выставления счетов. |
| пктобцексчанжератедате | Дата, на которую определяется Валюта ценообразования в валюте выставления счетов. |
| ентитлементид | Представляет идентификатор подписки Azure. |
| ентитлементдескриптион | Представляет имя идентификатора подписки Azure. |
| партнереарнедкредитперцентаже | Отображает Партнереарнедкредит для элемента строки. Заработанный кредит будет иметь значение 0 или 15 процентов |
