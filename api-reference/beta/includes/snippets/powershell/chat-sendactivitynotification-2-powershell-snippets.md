---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed193db6c27436faa07e3c22a05dcc5ee64e82e9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348834"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
    }
    ActivityType = "approvalRequired"
    PreviewText = @{
        Content = "Deployment requires your approval"
    }
    Recipient = @{
        "@odata.type" = "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient"
        UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
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