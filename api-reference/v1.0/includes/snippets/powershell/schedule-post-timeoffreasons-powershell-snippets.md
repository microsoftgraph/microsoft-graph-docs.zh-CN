---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18530d00cec940140957355be08821dee262d490
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124458"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Vacation"
    IconType = "plane"
    IsActive = $true
}

New-MgTeamScheduleTimeOffReason -TeamId $teamId -BodyParameter $params

```