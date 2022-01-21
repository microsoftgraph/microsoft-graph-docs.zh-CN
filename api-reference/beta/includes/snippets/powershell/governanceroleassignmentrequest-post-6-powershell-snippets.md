---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e75102265a534a1e833e2b9a2d970a3d4f69dd00
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113679"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RoleDefinitionId = "0e88fd18-50f5-4ee1-9104-01c3ed910065"
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
    SubjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6"
    AssignmentState = "Eligible"
    Type = "AdminExtend"
    Reason = "extend role assignment"
    Schedule = @{
        Type = "Once"
        StartDateTime = [System.DateTime]::Parse("2018-05-12T23:53:55.327Z")
        EndDateTime = [System.DateTime]::Parse("2018-08-10T23:53:55.327Z")
    }
}

New-MgPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params

```