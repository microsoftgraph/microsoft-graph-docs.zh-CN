---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83d029295e8e1d2168e79bb737d702083b416e10
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340939"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
    }
    ActivityType = "taskCreated"
    PreviewText = @{
        Content = "New Task Created"
    }
    TemplateParameters = @(
        @{
            Name = "taskId"
            Value = "Task 12322"
        }
    )
}

Send-MgUserTeamworkActivityNotification -UserId $userId -BodyParameter $params

```