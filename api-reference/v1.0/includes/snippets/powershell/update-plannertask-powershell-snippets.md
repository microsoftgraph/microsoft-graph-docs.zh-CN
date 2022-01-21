---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 820035fe31b62060a4082d4fd014b4724b3382a3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132269"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    Assignments = @{
        "Fbab97d0-4932-4511-b675-204639209557" = @{
            "@odata.type" = "#microsoft.graph.plannerAssignment"
            OrderHint = "N9917 U2883!"
        }
    }
    AppliedCategories = @{
        Category3 = $true
        Category4 = $false
    }
}

Update-MgPlannerTask -PlannerTaskId $plannerTaskId -BodyParameter $params

```