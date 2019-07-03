---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 424c66e5007789b7d078d60eb8f85a5734939a6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520905"
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