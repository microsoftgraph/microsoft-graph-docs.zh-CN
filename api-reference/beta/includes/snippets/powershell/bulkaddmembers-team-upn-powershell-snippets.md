---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2088e0b399b2e6530d4605e5ad85fbfba83aa129
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348884"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Values = @(
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('jacob@contoso.com')"
        }
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('alex@contoso.com')"
        }
    )
}

Add-MgTeamMember -TeamId $teamId -BodyParameter $params

```