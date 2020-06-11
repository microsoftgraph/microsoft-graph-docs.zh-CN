---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4667d868bf17c113d44ea0c90eef9452f31112a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681668"
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

await graphClient.Planner.Tasks["{task-id}"]
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerTask);

```