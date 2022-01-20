---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e2cbdf47762467487b54503be8891929a3bba9e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123330"
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

New-MgUserOutlookTask -UserId $userId -BodyParameter $params

```