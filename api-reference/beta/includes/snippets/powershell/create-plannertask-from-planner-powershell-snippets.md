---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fae2e24ef94cc0d3f68e2cac29a92a4197b04d63
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118584"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    PlanId = "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    BucketId = "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    Title = "Update client list"
    Assignments = @{
        "Fbab97d0-4932-4511-b675-204639209557" = @{
            "@odata.type" = "#microsoft.graph.plannerAssignment"
            OrderHint = " !"
        }
    }
}

New-MgPlannerTask -BodyParameter $params

```