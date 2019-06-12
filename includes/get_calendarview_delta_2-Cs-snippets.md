---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d27212649d395513c839454a9d624d861906b19
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.CalendarView.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .SkipToken("R0usmcCM996atia_s")
    .GetAsync();

```