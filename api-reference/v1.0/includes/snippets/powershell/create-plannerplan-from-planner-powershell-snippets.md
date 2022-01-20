---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4bf3e780bd156f6c967f7e10c6d9e835e05bb19
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092106"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    Owner = "ebf3b108-5234-4e22-b93d-656d7dae5874"
    Title = "title-value"
}

New-MgPlannerPlan -BodyParameter $params

```