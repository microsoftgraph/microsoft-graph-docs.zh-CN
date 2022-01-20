---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52f53c040849b68e5b180390b31e0245372d6275
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087690"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"
    DisplayName = "My Sample Team"
    Description = "My Sample Team’s Description"
    Members = @(
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
        }
    )
}

New-MgTeam -BodyParameter $params

```