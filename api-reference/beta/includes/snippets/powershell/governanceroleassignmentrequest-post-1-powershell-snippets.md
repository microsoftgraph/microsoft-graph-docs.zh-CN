---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85db90eef160e484c10c847cc25653a7396ff462
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113678"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RoleDefinitionId = "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d"
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
    SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
    AssignmentState = "Eligible"
    Type = "AdminAdd"
    Reason = "Assign an eligible role"
    Schedule = @{
        StartDateTime = [System.DateTime]::Parse("2018-05-12T23:37:43.356Z")
        EndDateTime = [System.DateTime]::Parse("2018-11-08T23:37:43.356Z")
        Type = "Once"
    }
}

New-MgPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params

```