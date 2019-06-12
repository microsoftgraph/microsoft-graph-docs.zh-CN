---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 940ac47faa59cdd42dafd03637bb8931454ca314
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.CalendarView.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .SkipToken("R0usmci39OQxqJrxK4")
    .GetAsync();

```