---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c720cdf1847ef1e846c9f0bb0f0a1c0aa26ad2f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111037"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    OriginalStartTimeZone = "originalStartTimeZone-value"
    OriginalEndTimeZone = "originalEndTimeZone-value"
    ResponseStatus = @{
        Response = ""
        Time = [System.DateTime]::Parse("datetime-value")
    }
    Recurrence = $null
    ReminderMinutesBeforeStart = 99
    IsOnlineMeeting = $true
    OnlineMeetingProvider = "teamsForBusiness"
    IsReminderOn = $true
    HideAttendees = $false
    Categories = @(
        "Red category"
    )
}

Update-MgUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```