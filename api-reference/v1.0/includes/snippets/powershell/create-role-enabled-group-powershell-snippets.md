---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c22a5efc3f2823e62457838e6f49ba51cdc32104
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095351"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Description = "Group assignable to a role"
    DisplayName = "Role assignable group"
    GroupTypes = @(
        "Unified"
    )
    IsAssignableToRole = $true
    MailEnabled = $true
    SecurityEnabled = $true
    MailNickname = "contosohelpdeskadministrators"
    "Owners@odata.bind" = @(
        "https://graph.microsoft.com/v1.0/users/99e44b05-c10b-4e95-a523-e2732bbaba1e"
    )
    "Members@odata.bind" = @(
        "https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0"
        "https://graph.microsoft.com/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e"
    )
}

New-MgGroup -BodyParameter $params

```