---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 559dea55bcd8f2801c1b67e96bdd9e988cda0ced
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500553"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEvent personAnnualEvent = new PersonAnnualEvent();
personAnnualEvent.allowedAudiences = EnumSet.of(AllowedAudiences.CONTACTS);

graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .patch(personAnnualEvent);

```