---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 439df2d34f631a3e8fa912adb44aa3a1d37a0025
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128604"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    SchedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"
    SharedOpenShift = @{
        Notes = "Inventory Management"
        OpenSlotCount = 5
        DisplayName = "Field shift"
        StartDateTime = [System.DateTime]::Parse("2018-10-04T00:58:45.340Z")
        EndDateTime = [System.DateTime]::Parse("2018-10-04T09:50:45.332Z")
        Theme = "white"
        Activities = @(
            @{
                IsPaid = $true
                StartDateTime = [System.DateTime]::Parse("2018-10-04T00:58:45.340Z")
                EndDateTime = [System.DateTime]::Parse("2018-10-04T01:58:45.340Z")
                Code = ""
                DisplayName = "Lunch"
            }
        )
    }
    DraftOpenShift = $null
}

Update-MgTeamScheduleOpenShift -TeamId $teamId -OpenShiftId $openShiftId -BodyParameter $params

```