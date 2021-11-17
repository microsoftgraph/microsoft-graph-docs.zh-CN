---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 658b7c1b53e648aab2828498d8a69bb6dfbc2370003940a1359a10dd50c2231e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333331"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEvent personAnnualEvent = new PersonAnnualEvent();
personAnnualEvent.type = PersonAnnualEventType.BIRTHDAY;
personAnnualEvent.date = new DateOnly(1900,1,1);

graphClient.me().profile().anniversaries()
    .buildRequest()
    .post(personAnnualEvent);

```