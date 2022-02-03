---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41125c3ad77c9efa38f431b063c3d5e5cbe0671a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345569"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    NotifyTeam = $true
    StartDateTime = [System.DateTime]::Parse("2018-10-08T00:00:00.000Z")
    EndDateTime = [System.DateTime]::Parse("2018-10-15T00:00:00.000Z")
}

Invoke-MgShareTeamSchedule -TeamId $teamId -BodyParameter $params

```