---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81e3e0787965e6b09ab55f3a3dc0c4d68ad9fa2e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101582"
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
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')"
            Roles = @(
                "owner"
            )
        }
    )
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```