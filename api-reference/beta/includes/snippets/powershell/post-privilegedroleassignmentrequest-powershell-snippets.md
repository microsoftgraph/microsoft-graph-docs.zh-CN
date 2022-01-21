---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abbb8fc8904db98831e570be9bf9fe59ac8274c6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136987"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    Duration = "2"
    Reason = "Activate the role for business purpose"
    TicketNumber = "234"
    TicketSystem = "system"
    Schedule = @{
        StartDateTime = [System.DateTime]::Parse("2018-02-08T02:35:17.903Z")
    }
    Type = "UserAdd"
    AssignmentState = "Active"
    RoleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}

New-MgPrivilegedRoleAssignmentRequest -BodyParameter $params

```