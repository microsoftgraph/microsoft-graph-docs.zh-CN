---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dd3b5c4d9507c842b436b2c1cd5aed801a8a478
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348833"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "text"
        Value = "Deployment Approvals Channel"
        WebUrl = "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    }
    ActivityType = "deploymentApprovalRequired"
    PreviewText = @{
        Content = "New deployment requires your approval"
    }
    Recipient = @{
        "@odata.type" = "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient"
        UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
    }
    TemplateParameters = @(
        @{
            Name = "deploymentId"
            Value = "6788662"
        }
    )
}

Send-MgChatActivityNotification -ChatId $chatId -BodyParameter $params

```