---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5638cd94cd6ed95cb7c98f46c7d88e82eec70de5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133109"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    Title = "title-value"
}

Update-MgPlannerPlan -PlannerPlanId $plannerPlanId -BodyParameter $params

```