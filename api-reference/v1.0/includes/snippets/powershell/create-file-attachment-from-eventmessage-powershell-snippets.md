---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa2455c8c41cd9fccbb70935b7afee71ff786e55
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111017"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "microsoft.graph.fileAttachment"
    Name = "name-value"
    ContentType = "contentType-value"
    IsInline = $false
    ContentLocation = "contentLocation-value"
    ContentBytes = "base64-contentBytes-value"
}

New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```