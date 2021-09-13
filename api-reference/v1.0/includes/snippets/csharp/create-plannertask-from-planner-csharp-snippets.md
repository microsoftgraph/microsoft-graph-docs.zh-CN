---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60040897b66e743e77abf29d1f1add1ac73e7753dfc192b19729daa534cd897a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333919"
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