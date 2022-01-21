---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25b3156470a43d7d2e9ce7e17e7a792580ea7da5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087691"
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
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')"
        }
    )
}

New-MgTeam -BodyParameter $params

```