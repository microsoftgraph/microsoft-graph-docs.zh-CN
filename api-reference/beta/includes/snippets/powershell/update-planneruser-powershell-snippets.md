---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6669c0c2b0e4ec56482384b441871ca3b0cb858
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118409"
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

Update-MgUserPlanner -UserId $userId -BodyParameter $params

```