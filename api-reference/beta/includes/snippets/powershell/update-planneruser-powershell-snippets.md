---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4579bab3ae3537c8de7f70ad3aa27645fbaddcdc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350498"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    FavoritePlanReferences = @{
        Jd8S5gOaFk2S8aWCIAJz42QAAxtD = @{
            "@odata.type" = "#microsoft.graph.plannerFavoritePlanReference"
            OrderHint = " !"
            PlanTitle = "Next Release Discussion"
        }
        "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" = $null
    }
    RecentPlanReferences = @{
        Jd8S5gOaFk2S8aWCIAJz42QAAxtD = @{
            "@odata.type" = "#microsoft.graph.plannerRecentPlanReference"
            LastAccessedDateTime = "2018-01-02T22:49:46.155Z"
            PlanTitle = "Next Release Discussion"
        }
    }
}

# A UPN can also be used as -UserId.
Update-MgUserPlanner -UserId $userId -BodyParameter $params

```