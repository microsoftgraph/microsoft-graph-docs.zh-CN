---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c17fe94b74e5e13e17b2d1eba3702f1e6694269
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136176"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "menu.txt"
    ContentBytes = "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}

New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params

```