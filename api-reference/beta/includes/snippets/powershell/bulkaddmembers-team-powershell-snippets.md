---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0984eff472775ebd7116b5d001d2174770e8df8b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348882"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Values = @(
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        }
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    )
}

Add-MgTeamMember -TeamId $teamId -BodyParameter $params

```