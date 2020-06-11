---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6f48ff8ca4596693dbc7d6ac6fae6333d0bdfb7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = new PlannerPlanDetails
{
    SharedWith = new PlannerUserIds
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"6463a5ce-2119-4198-9f2a-628761df4a62", "true"},
            {"d95e6152-f683-4d78-9ff5-67ad180fea4a", "false"}
        }
    },
    CategoryDescriptions = new PlannerCategoryDescriptions
    {
        Category1 = "Indoors",
        Category3 = null
    }
};

await graphClient.Planner.Plans["{plan-id}"].Details
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerPlanDetails);

```