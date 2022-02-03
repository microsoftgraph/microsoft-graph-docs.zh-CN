---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d102742454e60b93a1492e93ed149ef2536a153
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343888"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    }
    ActivityType = "reservationUpdated"
    PreviewText = @{
        Content = "You have moved up the queue"
    }
    Recipient = @{
        "@odata.type" = "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient"
        UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
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