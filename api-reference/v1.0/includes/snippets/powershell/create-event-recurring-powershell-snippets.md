---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57045e8343ae5c99d0cb3d8568f4724c14d68b3b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104192"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Let's go for lunch"
    Body = @{
        ContentType = "HTML"
        Content = "Does noon time work for you?"
    }
    Start = @{
        DateTime = "2017-09-04T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2017-09-04T14:00:00"
        TimeZone = "Pacific Standard Time"
    }
    Recurrence = @{
        Pattern = @{
            Type = "weekly"
            Interval = 1
            DaysOfWeek = @(
                "Monday"
            )
        }
        Range = @{
            Type = "endDate"
            StartDate = "2017-09-04"
            EndDate = "2017-12-31"
        }
    }
    Location = @{
        DisplayName = "Harry's Bar"
    }
    Attendees = @(
        @{
            EmailAddress = @{
                Address = "AdeleV@contoso.onmicrosoft.com"
                Name = "Adele Vance"
            }
            Type = "required"
        }
    )
    AllowNewTimeProposals = $true
}

New-MgUserEvent -UserId $userId -BodyParameter $params

```