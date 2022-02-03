---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c53c7959f06537c0ce86786438ac7637f8acd0cf
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346803"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Values = @(
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
            )
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        }
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    )
}

Add-MgTeamMember -TeamId $teamId -BodyParameter $params

```