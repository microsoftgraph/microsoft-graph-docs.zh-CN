---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f134c8a00f9478db866ce626cd7a791da253d3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130600"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Let's go for lunch"
    Body = @{
        ContentType = "HTML"
        Content = "Does noon work for you?"
    }
    Start = @{
        DateTime = "2017-04-15T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2017-04-15T14:00:00"
        TimeZone = "Pacific Standard Time"
    }
    Location = @{
        DisplayName = "Harry's Bar"
    }
    Attendees = @(
        @{
            EmailAddress = @{
                Address = "samanthab@contoso.onmicrosoft.com"
                Name = "Samantha Booth"
            }
            Type = "required"
        }
    )
    AllowNewTimeProposals = $true
    IsOnlineMeeting = $true
    OnlineMeetingProvider = "teamsForBusiness"
}

New-MgUserEvent -UserId $userId -BodyParameter $params

```