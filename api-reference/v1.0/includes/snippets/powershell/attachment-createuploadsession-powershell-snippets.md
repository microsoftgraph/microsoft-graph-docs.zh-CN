---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 363d74987791f668b5b4f1e414af2b057f959484
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342408"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AttachmentItem = @{
        AttachmentType = "file"
        Name = "flower"
        Size = 3483322
    }
}

# A UPN can also be used as -UserId.
New-MgUserMessageAttachmentUploadSession -UserId $userId -MessageId $messageId -BodyParameter $params

```