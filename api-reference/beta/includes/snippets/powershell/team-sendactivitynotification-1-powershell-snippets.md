---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 503c36503d84c0aec5edb81e6fbd9afc907876e1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343890"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/teams/{teamId}"
    }
    ActivityType = "pendingFinanceApprovalRequests"
    PreviewText = @{
        Content = "Internal spending team has a pending finance approval requests"
    }
    Recipient = @{
        "@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
        UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
    }
    TemplateParameters = @(
        @{
            Name = "pendingRequestCount"
            Value = "5"
        }
    )
}

Send-MgTeamActivityNotification -TeamId $teamId -BodyParameter $params

```