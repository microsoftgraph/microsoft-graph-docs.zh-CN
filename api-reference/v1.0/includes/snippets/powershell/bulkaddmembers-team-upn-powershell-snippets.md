---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b899fca95dbaafb831c46ed37656b57d1e021654
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346802"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Values = @(
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
            )
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
        }
        @{
            "@odata.type" = "microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('alex@contoso.com')"
        }
    )
}

Add-MgTeamMember -TeamId $teamId -BodyParameter $params

```