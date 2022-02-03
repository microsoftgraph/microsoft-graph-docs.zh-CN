---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfbc1b77471e2225d1c1666239304aab4b1fc5f2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343050"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    NewReminderTime = @{
        DateTime = "2016-10-19T10:37:00Z"
        TimeZone = "timeZone-value"
    }
}

# A UPN can also be used as -UserId.
Invoke-MgSnoozeUserEventReminder -UserId $userId -EventId $eventId -BodyParameter $params

```