---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3426bce9f413d16ea558825406ab24340e5cd0c6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500550"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEvent personAnnualEvent = new PersonAnnualEvent();
personAnnualEvent.type = PersonAnnualEventType.BIRTHDAY;
personAnnualEvent.date = new DateOnly(1900,1,1);

graphClient.me().profile().anniversaries()
    .buildRequest()
    .post(personAnnualEvent);

```