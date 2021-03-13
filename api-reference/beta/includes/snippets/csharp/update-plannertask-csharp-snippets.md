---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d3064f3a00e56fcf0a7cac090bcd96853fbb8f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789849"
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
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerTask);

```