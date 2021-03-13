---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af7b65d79a1f15a5660796ca3d66f72e4d7d97f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795807"
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

await graphClient.Planner.Plans["{plannerPlan-id}"].Details
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerPlanDetails);

```