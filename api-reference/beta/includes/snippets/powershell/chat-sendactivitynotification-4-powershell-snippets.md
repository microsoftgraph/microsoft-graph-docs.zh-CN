---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52026d946034fa207d558924efe54b6136427b5c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348835"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    }
    ActivityType = "taskCreated"
    PreviewText = @{
        Content = "New Task Created"
    }
    Recipient = @{
        "@odata.type" = "microsoft.graph.chatMembersNotificationRecipient"
        ChatId = "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
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