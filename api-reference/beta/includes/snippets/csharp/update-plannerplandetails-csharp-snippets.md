---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 614a8e71dee38b1a8d17c3c5115f0dac3dffed41
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573190"
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