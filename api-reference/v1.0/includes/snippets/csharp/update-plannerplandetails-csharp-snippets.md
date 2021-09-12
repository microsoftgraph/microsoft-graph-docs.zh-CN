---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 040c30e47c89be5cb147c9d0b482c185cfcfa5ab5eafcd1107e21983d76178ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904297"
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
    .Header("Prefer","return=representation")
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerPlanDetails);

```