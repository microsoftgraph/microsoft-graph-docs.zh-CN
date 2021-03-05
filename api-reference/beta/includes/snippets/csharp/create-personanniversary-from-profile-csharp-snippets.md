---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1367a6c7e6f034ebe39f1e2075578ca740e9242f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = new PersonAnnualEvent
{
    Type = PersonAnnualEventType.Birthday,
    Date = new Date(1980,1,8)
};

await graphClient.Me.Profile.Anniversaries
    .Request()
    .AddAsync(personAnnualEvent);

```