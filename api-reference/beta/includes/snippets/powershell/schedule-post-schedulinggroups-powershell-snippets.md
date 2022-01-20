---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65adce45078f53eedff5b89ba29dbf86439aeb23
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099001"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Cashiers"
    IsActive = $true
    UserIds = @(
        "c5d0c76b-80c4-481c-be50-923cd8d680a1"
        "2a4296b3-a28a-44ba-bc66-0274b9b95851"
    )
}

New-MgTeamScheduleSchedulingGroup -TeamId $teamId -BodyParameter $params

```