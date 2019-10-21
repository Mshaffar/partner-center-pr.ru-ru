---
title: Как рассчитывается полученный кредит от партнера | Центр партнеров
ms.topic: article
ms.date: 09/17/2019
description: Как рассчитывается процент полученного кредита плана Azure
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: eb0dd5ef22632a85ca0227cc9e988a88263e9ddf
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318769"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a>Как вычисляется кредитоспособный кредит (PEC) партнера


Партнеры, владеющие Круглосуточная эксплуатацией ИТ или всей среды Azure своих клиентов в CSP, получают с помощью PEC. PEC предоставляется в качестве части счета партнеру, имеющему прямую связь с корпорацией Майкрософт. Кредит вычисляется ежедневно и отражается в месячном счете. По умолчанию в CSP партнерам предоставляются необходимые права доступа к подписке клиента, позволяющие круглосуточно управлять ресурсами в подписке и управлять ими. Дополнительные способы, с помощью которых клиент может подготавливать доступ для передействующего партнера, описаны в следующем разделе.   


## <a name="important-eligibility-and-calculation-requirements"></a>Важные требования к допустимости и вычислениям:

- У партнера должно быть активное соглашение MPN и действующая роль с учетной записью C (RBAC) на основе правил для получения заработанного кредита для ресурсов Azure, которыми они управляют. Дополнительные сведения [допустимые роли RBAC]

- Косвенный поставщик будет иметь право на PEC, если они или их непрямое торговые посредники, или оба имеют Круглосуточная оперативный контроль и управление ресурсами Azure клиента в CSP.

- PEC связан с выставленным счетом за использование клиентской стороны Azure в CSP, управляемом партнером. 

- PEC доступен только партнерам в CSP, за которые взимается плата Майкрософт (косвенный поставщик и прямой счет).

- Подходящие службы: заработанный кредитный курс применяется ко всем ресурсам Azure 1PP Azure, указанным в прайс-списке. Существуют исключения, включая, но не ограниченные, 3PP и резервирование Azure.

- PEC вычисляется ежедневно и может быть просмотрен в ежедневном разведывательную файле. Партнер (поставщик или торговый посредник (через поставщика услуг) должен иметь доступ ко всему дню (круглосуточно), чтобы гарантировать получение PEC.

- PEC задается на уровне ресурсов Azure. Если у партнера есть допустимый доступ в подписке или на уровне группы ресурсов, каждый ресурс, который имеет роль до более высокой сущности, будет получать PEC. 

- PEC будет включен в ежемесячный счет партнера. В счете указана чистая оплата. Сведения отображаются в файле счета разведывательную.

Сведения о получении доступа к управлению подписками Azure и о том, как связать идентификатор MPN с ролями RBAC, см. в статье [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md).

Дополнительные сведения

- [План Azure — выставление счетов](azure-plan-billing.md)

- [Прейскурант для нового коммерческого опыта в CSP](azure-plan-price-list.md)