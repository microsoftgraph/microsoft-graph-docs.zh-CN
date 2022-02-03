---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cffc76903a975e0e457c21ebe88499980fdf32c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351740"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Subject = "Shop for dinner"
    StartDateTime = @{
        DateTime = "2016-04-23T18:00:00"
        TimeZone = "Pacific Standard Time"
    }
    DueDateTime = @{
        DateTime = "2016-04-25T13:00:00"
        TimeZone = "Pacific Standard Time"
    }
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTaskFolderTask -UserId $userId -OutlookTaskFolderId $outlookTaskFolderId -BodyParameter $params

```