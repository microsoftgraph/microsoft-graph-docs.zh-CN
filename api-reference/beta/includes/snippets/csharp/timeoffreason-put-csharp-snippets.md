---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 424c66e5007789b7d078d60eb8f85a5734939a6a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReason = new TimeOffReason
{
    DisplayName = "Vacation",
    IconType = TimeOffReasonIconType.Plane,
    IsActive = true
};

await graphClient.Teams["{teamId}"].Schedule.TimeOffReasons["{timeOffReasonId}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(timeOffReason);

```