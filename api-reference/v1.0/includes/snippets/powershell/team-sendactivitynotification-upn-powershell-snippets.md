---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a086b312a824d475d2c5932a500ec3efe6938deb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339929"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    }
    ActivityType = "reservationUpdated"
    PreviewText = @{
        Content = "You have moved up the queue"
    }
    Recipient = @{
        "@odata.type" = "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient"
        UserId = "jacob@contoso.com"
    }
    TemplateParameters = @(
        @{
            Name = "reservationId"
            Value = "TREEE433"
        }
        @{
            Name = "currentSlot"
            Value = "23"
        }
    )
}

Send-MgTeamActivityNotification -TeamId $teamId -BodyParameter $params

```