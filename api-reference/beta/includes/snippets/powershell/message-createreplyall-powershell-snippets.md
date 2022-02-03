---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c8a2d1463996e3c724dcf1939a5b087cc97788b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341629"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        Attachments = @(
            @{
                "@odata.type" = "#microsoft.graph.fileAttachment"
                Name = "guidelines.txt"
                ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
            }
        )
    }
    Comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name."
}

# A UPN can also be used as -UserId.
New-MgUserMessageReplyAll -UserId $userId -MessageId $messageId -BodyParameter $params

```