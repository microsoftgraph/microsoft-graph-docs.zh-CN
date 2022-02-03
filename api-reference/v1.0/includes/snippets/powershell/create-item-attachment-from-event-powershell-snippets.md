---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d033f7e89b71d548efa2b3b6aaa8bd45b24a2cc4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351606"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "#microsoft.graph.itemAttachment"
    Name = "Holiday event"
    Item = @{
        "@odata.type" = "microsoft.graph.event"
        Subject = "Discuss gifts for children"
    }
}

# A UPN can also be used as -UserId.
New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params

```