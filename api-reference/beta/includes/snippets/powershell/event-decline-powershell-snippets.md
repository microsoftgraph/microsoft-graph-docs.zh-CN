---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65378e735313183f0fcf12a660bc1e19224735f7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341714"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Comment = "I won't be able to make this week. How about next week?"
    SendResponse = $true
    ProposedNewTime = @{
        Start = @{
            DateTime = "2019-12-02T18:00:00"
            TimeZone = "Pacific Standard Time"
        }
        End = @{
            DateTime = "2019-12-02T19:00:00"
            TimeZone = "Pacific Standard Time"
        }
    }
}

# A UPN can also be used as -UserId.
Invoke-MgDeclineUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```