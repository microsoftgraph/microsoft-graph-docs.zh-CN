---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 545b577c5322bbeea00a7a5955f8287ff805e65b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099458"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "#microsoft.graph.referenceAttachment"
    Name = "Personal pictures"
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics"
    ProviderType = "oneDriveConsumer"
    Permission = "Edit"
    IsFolder = "True"
}

New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```