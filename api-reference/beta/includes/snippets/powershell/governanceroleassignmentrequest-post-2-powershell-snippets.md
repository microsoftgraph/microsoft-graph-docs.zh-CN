---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daaa9632af4cd3e82bff6a449d254d912f448b44
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113676"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RoleDefinitionId = "8b4d1d51-08e9-4254-b0a6-b16177aae376"
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
    SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
    AssignmentState = "Active"
    Type = "UserAdd"
    Reason = "Activate the owner role"
    Schedule = @{
        Type = "Once"
        StartDateTime = [System.DateTime]::Parse("2018-05-12T23:28:43.537Z")
        Duration = "PT9H"
    }
    LinkedEligibleRoleAssignmentId = "e327f4be-42a0-47a2-8579-0a39b025b394"
}

New-MgPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params

```