---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d697243d36debb29fb2a13093f5c98e4f05a0cd3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479831"
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

await graphClient.Planner.Plans["xqQg5FS2LkCp935s-FIFm2QAFkHM"].Details
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerPlanDetails);

```