---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a393d1d463c5c5567fbcbc011e45515a6a856fe7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedulingGroup = new SchedulingGroup
{
    DisplayName = "Cashiers",
    IsActive = true,
    UserIds = new List<String>()
    {
        "c5d0c76b-80c4-481c-be50-923cd8d680a1",
        "2a4296b3-a28a-44ba-bc66-0274b9b95851"
    }
};

await graphClient.Teams["{teamId}"].Schedule.SchedulingGroups
    .Request()
    .AddAsync(schedulingGroup);

```