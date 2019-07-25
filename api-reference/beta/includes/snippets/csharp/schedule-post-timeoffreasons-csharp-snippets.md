---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bffd51984e24f373ca388b5152b6d58d7267c7c2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718141"
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