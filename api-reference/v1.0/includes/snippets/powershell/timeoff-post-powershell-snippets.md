---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bb262f80d8d6859c03bd8ffe06503cd988a1078
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110823"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    UserId = "c5d0c76b-80c4-481c-be50-923cd8d680a1"
    SharedTimeOff = @{
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7"
        StartDateTime = [System.DateTime]::Parse("2019-03-11T07:00:00Z")
        EndDateTime = [System.DateTime]::Parse("2019-03-12T07:00:00Z")
        Theme = "white"
    }
    DraftTimeOff = @{
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7"
        StartDateTime = [System.DateTime]::Parse("2019-03-11T07:00:00Z")
        EndDateTime = [System.DateTime]::Parse("2019-03-12T07:00:00Z")
        Theme = "pink"
    }
}

New-MgTeamScheduleTimeOff -TeamId $teamId -BodyParameter $params

```