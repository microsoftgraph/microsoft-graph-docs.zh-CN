---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f521a22dda77ecb3aa169e2dff177c2e4c97da6c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "name-value"
};

await graphClient.Me.CalendarGroups["{id}"]
    .Request()
    .UpdateAsync(calendarGroup);

```