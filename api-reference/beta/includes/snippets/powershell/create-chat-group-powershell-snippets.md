---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c04e2d438d99b800d370242c44f762a9282b3b5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090962"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    ChatType = "group"
    Topic = "Group chat title"
    Members = @(
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
        }
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
        }
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"
        }
    )
}

New-MgChat -BodyParameter $params

```