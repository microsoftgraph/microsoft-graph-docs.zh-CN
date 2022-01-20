---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c72591850be0ca3e8b069c3de7e8e5544e4294c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113677"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RoleDefinitionId = "70521f3e-3b95-4e51-b4d2-a2f485b02103"
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
    SubjectId = "1566d11d-d2b6-444a-a8de-28698682c445"
    AssignmentState = "Eligible"
    Type = "AdminUpdate"
    Schedule = @{
        Type = "Once"
        StartDateTime = [System.DateTime]::Parse("2018-03-08T05:42:45.317Z")
        EndDateTime = [System.DateTime]::Parse("2018-06-05T05:42:31.000Z")
    }
}

New-MgPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params

```