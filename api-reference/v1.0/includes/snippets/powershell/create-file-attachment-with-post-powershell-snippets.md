---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc2b5d732abefd7d52a5120f154213542a8cf7a6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341805"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Post = @{
        Body = @{
            ContentType = "text"
            Content = "Which quarter does that file cover? See my attachment."
        }
        Attachments = @(
            @{
                "@odata.type" = "#microsoft.graph.fileAttachment"
                Name = "Another file as attachment"
                ContentBytes = "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
            }
        )
    }
}

Invoke-MgReplyGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```