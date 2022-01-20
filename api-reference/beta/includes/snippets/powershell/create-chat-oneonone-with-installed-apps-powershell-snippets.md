---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61a5563692464a6798462d639b9fa250c061dd05
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090964"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    ChatType = "oneOnOne"
    Members = @(
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
        }
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
        }
    )
    InstalledApps = @(
        @{
            "TeamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4"
        }
    )
}

New-MgChat -BodyParameter $params

```