---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c3873caf3061fe8fd233c36229940bcb57460d9e4ca3419a2d73c820ffa0f9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = new PlannerTask
{
    Assignments = new PlannerAssignments
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"fbab97d0-4932-4511-b675-204639209557", "{\"@odata.type\":\"#microsoft.graph.plannerAssignment\",\"orderHint\":\"N9917 U2883!\"}"}
        }
    },
    AppliedCategories = new PlannerAppliedCategories
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"category3", "true"},
            {"category4", "false"}
        }
    }
};

await graphClient.Planner.Tasks["{plannerTask-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerTask);

```