---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77e68a3d50a0ecbd21991bce1abc51e5acf5986e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339930"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

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
}

Send-MgUserTeamworkActivityNotification -UserId $userId -BodyParameter $params

```