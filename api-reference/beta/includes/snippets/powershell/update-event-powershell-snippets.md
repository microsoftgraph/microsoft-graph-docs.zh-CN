---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cc83bd63b11773cd6fb2d00e30ea6ef438d6185
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349997"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    OriginalStartTimeZone = "originalStartTimeZone-value"
    OriginalEndTimeZone = "originalEndTimeZone-value"
    ResponseStatus = @{
        Response = ""
        Time = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
    }
    Recurrence = $null
    Uid = "iCalUId-value"
    ReminderMinutesBeforeStart = 99
    IsOnlineMeeting = $true
    OnlineMeetingProvider = "teamsForBusiness"
    IsReminderOn = $true
    HideAttendees = $false
    Categories = @(
        "Red category"
    )
}

# A UPN can also be used as -UserId.
Update-MgUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```