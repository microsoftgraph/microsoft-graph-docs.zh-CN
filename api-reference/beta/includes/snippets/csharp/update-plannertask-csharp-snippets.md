---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af57b3e69c16dbae6a780cfde701d7ab991bb7b3
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573166"
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