---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1686519878848986631e705daca97fa9492ea966
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350680"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "menu.txt"
    ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTaskAttachment -UserId $userId -OutlookTaskId $outlookTaskId -BodyParameter $params

```