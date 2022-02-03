---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbe6807d24035604eecae5a1468b2db142c076dc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343759"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    NewReminderTime = @{
        DateTime = "dateTime-value"
        TimeZone = "timeZone-value"
    }
}

# A UPN can also be used as -UserId.
Invoke-MgSnoozeUserEventReminder -UserId $userId -EventId $eventId -BodyParameter $params

```