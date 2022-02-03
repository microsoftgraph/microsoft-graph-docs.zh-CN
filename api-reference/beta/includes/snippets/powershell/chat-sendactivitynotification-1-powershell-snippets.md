---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3d234a08c9168d52c2056977307078ee7db576b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348836"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/chats/{chatId}"
    }
    ActivityType = "taskCreated"
    PreviewText = @{
        Content = "New Task Created"
    }
    Recipient = @{
        "@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
        UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
    }
    TemplateParameters = @(
        @{
            Name = "taskId"
            Value = "Task 12322"
        }
    )
}

Send-MgChatActivityNotification -ChatId $chatId -BodyParameter $params

```