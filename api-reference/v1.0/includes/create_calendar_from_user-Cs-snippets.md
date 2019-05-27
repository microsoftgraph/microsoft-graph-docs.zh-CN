---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e5669575a61028f928f917d8180b6db08f8a2e1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456009"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Volunteer"
};

await graphClient.Me.Calendars
    .Request()
    .AddAsync(calendar);

```