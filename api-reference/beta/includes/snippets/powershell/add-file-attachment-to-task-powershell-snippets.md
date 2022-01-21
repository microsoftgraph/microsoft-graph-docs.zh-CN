---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc09c0311152bc48cf99b0efe864e3edfe807a97
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112676"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "menu.txt"
    ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}

New-MgUserOutlookTaskAttachment -UserId $userId -OutlookTaskId $outlookTaskId -BodyParameter $params

```