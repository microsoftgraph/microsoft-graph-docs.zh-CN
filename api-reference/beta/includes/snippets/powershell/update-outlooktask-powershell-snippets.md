---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2621f8fa7a155bd9368c3bad8c5291c8fd66c93e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350587"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DueDateTime = @{
        DateTime = "2016-05-06T16:00:00"
        TimeZone = "Eastern Standard Time"
    }
}

# A UPN can also be used as -UserId.
Update-MgUserOutlookTask -UserId $userId -OutlookTaskId $outlookTaskId -BodyParameter $params

```