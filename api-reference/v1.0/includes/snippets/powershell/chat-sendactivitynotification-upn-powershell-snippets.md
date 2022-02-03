---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d23865df1e5d37f2c2c88b1fa366b87841e1c3e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339572"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}"
    }
    ActivityType = "approvalRequired"
    PreviewText = @{
        Content = "Deployment requires your approval"
    }
    Recipient = @{
        "@odata.type" = "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient"
        UserId = "jacob@contoso.com"
    }
    TemplateParameters = @(
        @{
            Name = "approvalTaskId"
            Value = "2020AAGGTAPP"
        }
    )
}

Send-MgChatActivityNotification -ChatId $chatId -BodyParameter $params

```