---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32fc4dcda5e260715c88f36088ae8fca838edb8c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347737"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Comment = "comment-value"
    ToRecipients = @(
        @{
            EmailAddress = @{
                Name = "name-value"
                Address = "address-value"
            }
        }
    )
}

Invoke-MgForwardGroupThreadPost -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -BodyParameter $params

```