---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 606895c0939e02dabf5d931357b8c157c22d5400
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117121"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    OrderHintsByAssignee = @{
        "Aaa27244-1db4-476a-a5cb-004607466324" = "8566473P 957764Jk!"
    }
}

Update-MgPlannerTaskAssignedToTaskBoardFormat -PlannerTaskId $plannerTaskId -BodyParameter $params

```