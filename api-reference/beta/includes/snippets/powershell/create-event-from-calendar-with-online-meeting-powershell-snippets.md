---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a85d4795f05bcae3c42fbab84d5e3c3f018d756
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351886"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Let's go for lunch"
    Body = @{
        ContentType = "HTML"
        Content = "Does next month work for you?"
    }
    Start = @{
        DateTime = "2019-03-10T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2019-03-10T14:00:00"
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
    IsOnlineMeeting = $true
    OnlineMeetingProvider = "teamsForBusiness"
}

# A UPN can also be used as -UserId.
New-MgUserCalendarEvent -UserId $userId -CalendarId $calendarId -BodyParameter $params

```