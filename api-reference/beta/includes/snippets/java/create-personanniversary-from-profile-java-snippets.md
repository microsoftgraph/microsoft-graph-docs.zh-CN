---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e722c0f866a366dbc5a1b8a4288b148c434fbaf2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964592"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnniversary personAnniversary = new PersonAnniversary();
personAnniversary.type = AnniversaryType.BIRTHDAY;
personAnniversary.date = new DateOnly(1900,1,1);

graphClient.me().profile().anniversaries()
    .buildRequest()
    .post(personAnniversary);

```