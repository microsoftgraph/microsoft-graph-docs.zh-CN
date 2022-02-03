---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9414da92ef4bdfbd3f985c2783fd1c0407fa493
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351207"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "#Microsoft.OutlookServices.ItemAttachment"
    Name = "name-value"
    Item = @{
        "@odata.type" = "microsoft.graph.message"
    }
}

# A UPN can also be used as -UserId.
New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params

```