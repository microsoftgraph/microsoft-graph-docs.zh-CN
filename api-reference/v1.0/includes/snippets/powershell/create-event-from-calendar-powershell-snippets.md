---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6343fb1695536ae0585edd42712ef973db7f6c13
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115169"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Let's go for lunch"
    Body = @{
        ContentType = "HTML"
        Content = "Does mid month work for you?"
    }
    Start = @{
        DateTime = "2019-03-15T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2019-03-15T14:00:00"
        TimeZone = "Pacific Standard Time"
    }
    Location = @{
        DisplayName = "Harry's Bar"
    }
    Attendees = @(
        @{
            EmailAddress = @{
                Address = "adelev@contoso.onmicrosoft.com"
                Name = "Adele Vance"
            }
            Type = "required"
        }
    )
    TransactionId = "7E163156-7762-4BEB-A1C6-729EA81755A7"
}

New-MgUserCalendarEvent -UserId $userId -CalendarId $calendarId -BodyParameter $params

```