---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fe3cf231c6920844235e5ccea0c3c453bdae9e8
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = new PlannerTask
{
    PlanId = "xqQg5FS2LkCp935s-FIFm2QAFkHM",
    BucketId = "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
    Title = "Update client list",
    Assignments = new PlannerAssignments
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"fbab97d0-4932-4511-b675-204639209557", "{\"@odata.type\":\"#microsoft.graph.plannerAssignment\",\"orderHint\":\" !\"}"}
        }
    }
};

await graphClient.Planner.Tasks
    .Request()
    .AddAsync(plannerTask);

```