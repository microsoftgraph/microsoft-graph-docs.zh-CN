---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00f0d9106cd5bbe7f291b7e07523559b96af2adf
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220270"
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
        "@odata.type" = "microsoft.graph.teamMembersNotificationRecipient"
        TeamId = "e8bece96-d393-4b9b-b8da-69cedef1a7e7"
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