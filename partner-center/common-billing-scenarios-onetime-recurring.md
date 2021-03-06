---
title: Выставление счетов за одноразовые & повторяющихся покупок
ms.topic: article
ms.date: 05/05/2020
description: Ознакомьтесь с примерами выставления счетов центра партнеров за разовые и выберите повторяющиеся покупки. при покупке подписки, добавлении дополнительных подписок, добавлении или удалении рабочих мест.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: выставление счетов, оплата, одноразовая покупка, повторная покупка, подписки, рабочие места
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2c3467fdbe8457a7068a49000bd635b7c464cf29
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908206"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Сценарии выставления счетов центра партнеров для одноразовых и выбора повторяющихся покупок

**Соответствующие роли**

- Агент по администрированию
- Администратор выставления счетов
- Агент службы технической поддержки
- Агент по продажам

В этих примерах [распространенные сценарии выставления счетов](common-billing-scenarios.md) применяются к [одноразовым и выбираются повторяющиеся платежи](one-time-and-recurring-billing.md) в центре партнеров.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Приобретите подписку и добавьте рабочее место в тот же день

В сценарии 1 вы приобретаете подписку 11 июня по 4 долл. США за единицу. Позже в тот же день вы приобретаете еще одну такую подписку по той же цене.

Файл сверки будет содержать следующее:

- 4 долл. США — платеж за период обслуживания с 10 июня по 9 июля.
- –4,00 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 11 по 11 июня. Это период, когда у вас была 1 лицензия. Расчет = (месячная цена / всего дней в периоде обслуживания) x количество дней в периоде обслуживания с пропорциональным перерасчетом x количество лицензий = (4 / 30) x 30 x 1 =4,00.
- 8,00 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 10 июня по 9 июля. Это период, когда у вас были 2 лицензии. Расчет = (4 / 30) x 30 x 2 = 8,00.

|**Дата покупки**   |**Начало платежа** |**Завершение платежа**  |**Цена за единицу**  |**Склад**  |**Сумма** |**Charge Type** (Тип платежей) |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 долл. США                |1                 |4 долл. США            |Создать         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 долл. США        |1        | –4 долл. США       |addQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 долл. США        | 2      |8 долл. США         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Приобретите подписку и добавьте дополнительные подписки позже

В сценарии 2 вы приобретаете подписку 11 июня по 4 долл. США за единицу, а 12 июня вы приобретаете еще одну подписку на тот же продукт по той же цене.

Файл сверки будет содержать следующее:

- 4 долл. США — платеж за период обслуживания с 10 июня по 9 июля.
- –3,87 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 11 по 12 июня. Это период, когда у вас была 1 лицензия. Расчет = (месячная цена / всего дней в периоде обслуживания) x количество дней в периоде обслуживания с пропорциональным перерасчетом x количество лицензий = (4 / 30) x 29 x 1 =3,87.
- 7,74 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 12 июня по 9 июля. Это период, когда у вас были 2 лицензии. Расчет = (4 / 30) x 29 x 2 = 7,74.

|**Дата покупки**   |**Начало платежа** |**Завершение платежа**  |**Цена за единицу**  |**Склад**  |**Сумма** |**Charge Type** (Тип платежей) |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (у вас одна лицензия)     |10.06.2019   |09.07.2019         |4 долл. США         |1        |4 долл. США            |Создать         |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 долл. США        |1        | –3,87 долл. США       |addQuantity           |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 долл. США        | 2      |7,74 долл. США       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Приобрести подписку и удалить рабочее место в тот же день

В сценарии 3 вы приобретаете две подписки на один и тот же продукт 11 июня по 4 долл. США за единицу. Позже в тот же день вы удаляете одно из рабочих мест.  

Файл сверки будет содержать следующее:

- 8 долл. США — платеж за две лицензии за период обслуживания с 10 июня по 9 июля.
- –8,00 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 11 по 11 июня. Это период, когда у вас были 2 лицензии. Расчет = (месячная цена / всего дней в периоде обслуживания) x количество дней в периоде обслуживания с пропорциональным перерасчетом x количество лицензий = (4 / 30) x 30 x 2 =8,00.
- 4,00 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 11 июня по 9 июля. Это период, когда у вас была 1 лицензия. Расчет = (4 / 30) x 30 x 1 = 4,00.

|**Дата покупки**   |**Начало платежа** |**Завершение платежа**  |**Цена за единицу**  |**Склад**  |**Сумма** |**Charge Type** (Тип платежей) |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 долл. США                |2                 |8 долл. США            |Создать         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 долл. США        |2        | -8 долл. США       |removeQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 долл. США        | 1      |4 долл. США         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Приобретение подписки и удаление рабочих мест позже

В сценарии 4 вы приобретаете 2 подписки по 4 долл. США за единицу 11 июня, а 12 июня вы удаляете одно из рабочих мест.

Файл сверки будет содержать следующее:

- 8 долл. США — платеж за период обслуживания с 10 июня по 9 июля.
- –7,74 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 11 по 12 июня. Это период, когда у вас были 2 лицензии. Расчет = (месячная цена / всего дней в периоде обслуживания) x количество дней в периоде обслуживания с пропорциональным перерасчетом x количество лицензий = (4 / 30) x 29 x 2 =7,74.
- 3,87 долл. США — платеж с пропорциональным перерасчетом за период обслуживания с 12 июня по 9 июля. Это период, когда у вас была 1 лицензия. Расчет = (4 / 30) x 29 x 1 = 3,87.

|**Дата покупки**   |**Начало платежа** |**Завершение платежа**  |**Цена за единицу**  |**Склад**  |**Сумма** |**Charge Type** (Тип платежей) |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (у вас 2 лицензии)     |10.06.2019   |09.07.2019         |4 долл. США         |2        |8 долл. США       |Создать       |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 долл. США        |2        | –7,74 долл. США       |removeQuantity           |
|12.06.2019 (у вас 1 лицензия)    | 10.06.2019    |09.07.2019   |4 долл. США    |1      |3,87 долл. США    |removeQuantity |
