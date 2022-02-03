---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d091ff3190ca327fc8403f5516206574a9b61775
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340371"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AttachmentItem = @{
        AttachmentType = "file"
        Name = "scenary"
        Size = 7208534
        IsInline = $true
        ContentId = "my_inline_picture"
    }
}

# A UPN can also be used as -UserId.
New-MgUserMessageAttachmentUploadSession -UserId $userId -MessageId $messageId -BodyParameter $params

```