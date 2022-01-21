---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca7af002d71f63ee93f693c1bd181c451714f05f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131565"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#Microsoft.Graph.channel"
    MembershipType = "private"
    DisplayName = "My First Private Channel"
    Description = "This is my first private channels"
    Members = @(
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('jacob@contoso.com')"
            Roles = @(
                "owner"
            )
        }
    )
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```