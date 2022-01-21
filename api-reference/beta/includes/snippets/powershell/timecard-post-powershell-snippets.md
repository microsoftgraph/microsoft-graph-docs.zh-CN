---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce7bd9056fb0c2b89d751bdd7904ec0317e0d1ec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129290"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    OnBehalfOfUserId = "a3601044-a1b5-438e-b742-f78d01d68a67"
    ClockInEvent = @{
        DateTime = [System.DateTime]::Parse("2019-03-18T00:00:00.000Z")
        AtApprovedLocation = $true
        Notes = @{
            Content = "Started late due to traffic in CA 237"
            ContentType = "text"
        }
    }
    Notes = @{
        Content = "8 To 5 Inventory management"
        ContentType = "text"
    }
    Breaks = @(
        @{
            BreakId = "string"
            Notes = @{
                Content = "Lunch break"
                ContentType = "text"
            }
            Start = @{
                DateTime = [System.DateTime]::Parse("2019-03-18T02:00:00.000Z")
                AtApprovedLocation = $true
                Notes = @{
                    Content = "Reduced break to make up for lost time"
                    ContentType = "text"
                }
            }
        }
    )
}

New-MgTeamScheduleTimeCard -TeamId $teamId -BodyParameter $params

```