---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edae729931aa00c987b01e6f97db9402ac3097d8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445171"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
    }
    ActivityType = "pendingFinanceApprovalRequests"
    PreviewText = @{
        Content = "Internal spending team has a pending finance approval requests"
    }
    Recipients = @(
        @{
            "@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
            UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
        }
        @{
            "@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
            UserId = "ab88234e-0874-477c-9638-d144296ed04f"
        }
        @{
            "@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
            UserId = "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    )
    TemplateParameters = @(
        @{
            Name = "pendingRequestCount"
            Value = "5"
        }
    )
}

Send-MgTeamworkActivityNotificationToRecipient -BodyParameter $params

```