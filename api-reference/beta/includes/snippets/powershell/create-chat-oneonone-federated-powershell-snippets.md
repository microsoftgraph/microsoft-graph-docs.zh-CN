---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a00a75dff135c9236142c57828f92fe0c73068d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436850"
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
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
        }
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            Roles = @(
                "owner"
            )
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
            TenantId = "4dc1fe35-8ac6-4f0d-904a-7ebcd364bea1"
        }
    )
}

New-MgChat -BodyParameter $params

```