---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9952f8c24e808b356650f561fde4ec3e299c7ee9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345583"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Comment = "I may not be able to make this week. How about next week?"
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
Invoke-MgAcceptUserEventTentatively -UserId $userId -EventId $eventId -BodyParameter $params

```