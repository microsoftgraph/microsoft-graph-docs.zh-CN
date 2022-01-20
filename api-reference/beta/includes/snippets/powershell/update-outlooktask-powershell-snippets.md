---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7eb690e56624c42fcd4a58e61b8d9050286d3cd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123351"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DueDateTime = @{
        DateTime = "2016-05-06T16:00:00"
        TimeZone = "Eastern Standard Time"
    }
}

Update-MgUserOutlookTask -UserId $userId -OutlookTaskId $outlookTaskId -BodyParameter $params

```