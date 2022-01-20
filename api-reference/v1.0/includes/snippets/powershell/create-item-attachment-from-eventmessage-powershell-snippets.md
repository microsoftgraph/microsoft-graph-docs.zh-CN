---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13b548a9f64317957c404c875e856eb6d8df19d6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111019"
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

New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params

```