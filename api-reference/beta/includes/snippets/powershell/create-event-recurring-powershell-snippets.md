---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5905fd24f63334a2b5bdab799fa2fd260820a47d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350734"
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
}

# A UPN can also be used as -UserId.
New-MgUserEvent -UserId $userId -BodyParameter $params

```