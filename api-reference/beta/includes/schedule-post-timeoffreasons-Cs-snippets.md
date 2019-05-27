---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bffd51984e24f373ca388b5152b6d58d7267c7c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReason = new TimeOffReason
{
    DisplayName = "Vacation",
    IconType = TimeOffReasonIconType.Plane,
    IsActive = true
};

await graphClient.Teams["{teamId}"].Schedule.TimeOffReasons
    .Request()
    .AddAsync(timeOffReason);

```