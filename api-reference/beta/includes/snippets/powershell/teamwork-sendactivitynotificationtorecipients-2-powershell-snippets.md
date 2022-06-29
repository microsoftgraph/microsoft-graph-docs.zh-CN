---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 237d5c2e291e9154460f6a284eed7b6699b78a82
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445169"
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
    TemplateParameters = @(
        @{
            Name = "deploymentId"
            Value = "6788662"
        }
    )
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
}

Send-MgTeamworkActivityNotificationToRecipient -BodyParameter $params

```