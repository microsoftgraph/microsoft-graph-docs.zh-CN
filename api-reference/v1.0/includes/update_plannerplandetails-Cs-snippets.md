---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17b4b31d4a02f09e5c08b98ac5d1816aad629447
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = new PlannerPlanDetails
{
    SharedWith = new PlannerUserIds
    {
        6463a5ce-2119-4198-9f2a-628761df4a62 = true,
        D95e6152-f683-4d78-9ff5-67ad180fea4a = false
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