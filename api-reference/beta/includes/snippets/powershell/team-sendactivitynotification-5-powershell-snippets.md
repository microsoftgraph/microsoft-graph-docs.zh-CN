---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90e016eeb4e577797c140081b3aed0052dd965c3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343891"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    }
    ActivityType = "pendingFinanceApprovalRequests"
    PreviewText = @{
        Content = "Internal spending team has a pending finance approval requests"
    }
    Recipient = @{
        "@odata.type" = "microsoft.graph.channelMembersNotificationRecipient"
        TeamId = "e8bece96-d393-4b9b-b8da-69cedef1a7e7"
        ChannelId = "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"
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