---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba6c9af1d3d735f3a2f3a674374d62d526a9154c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351730"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Subject = "Shop for children's weekend"
    StartDateTime = @{
        DateTime = "2016-05-03T09:00:00"
        TimeZone = "Eastern Standard Time"
    }
    DueDateTime = @{
        DateTime = "2016-05-05T16:00:00"
        TimeZone = "Eastern Standard Time"
    }
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTask -UserId $userId -BodyParameter $params

```