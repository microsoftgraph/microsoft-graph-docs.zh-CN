---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65ea625aeb2a08b63235135fbba4104519aea3a9
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093570"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = new PlannerPlan
{
    Container = new PlannerPlanContainer
    {
        Url = "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874"
    },
    Title = "title-value"
};

await graphClient.Planner.Plans
    .Request()
    .AddAsync(plannerPlan);

```