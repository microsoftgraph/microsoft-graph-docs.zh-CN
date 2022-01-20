---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ebcaddd6dc28f9ae62d54c81b1aa94f437a7ec4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113675"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RoleDefinitionId = "65bb4622-61f5-4f25-9d75-d0e20cf92019"
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
    SubjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6"
    AssignmentState = "Eligible"
    Type = "AdminRemove"
}

New-MgPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params

```