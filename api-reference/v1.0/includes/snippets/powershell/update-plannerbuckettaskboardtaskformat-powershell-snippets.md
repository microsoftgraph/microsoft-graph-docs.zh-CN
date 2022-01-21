---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7a7d04b62dab5548c40c9b13a88d94b0b6619ab
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092050"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    OrderHint = "A6673H Ejkl!"
}

Update-MgPlannerTaskBucketTaskBoardFormat -PlannerTaskId $plannerTaskId -BodyParameter $params

```