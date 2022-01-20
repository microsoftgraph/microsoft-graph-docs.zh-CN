---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac199c2ff7f636f33637d568ed30572784363ef
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097727"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "smile"
    ContentBytes = "R0lGODdhEAYEAA7"
}

New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```