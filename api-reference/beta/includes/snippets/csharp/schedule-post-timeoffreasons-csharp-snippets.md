---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bffd51984e24f373ca388b5152b6d58d7267c7c2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615792"
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