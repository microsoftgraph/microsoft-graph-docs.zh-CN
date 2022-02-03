---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f73b0e6560e5c3983ab3badc8fe08f476a1b555
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339722"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Post = @{
        Body = @{
            ContentType = "html"
            Content = "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
        }
        Extensions = @(
            @{
                "@odata.type" = "microsoft.graph.openTypeExtension"
                ExtensionName = "Com.Contoso.HR"
                CompanyName = "Contoso"
                ExpirationDate = "2015-07-03T13:04:00.000Z"
                TopPicks = @(
                    "Employees only"
                    "Add spouse or guest"
                    "Add family"
                )
            }
        )
    }
}

Invoke-MgReplyGroupThreadPost -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -BodyParameter $params

```