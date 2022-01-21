---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 414fa349cbf543b97013fc82dbb7efe0835b026d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113680"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RoleDefinitionId = "bc75b4e6-7403-4243-bf2f-d1f6990be122"
    ResourceId = "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735"
    SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
    AssignmentState = "Active"
    Type = "UserRemove"
    Reason = "Deactivate the role"
    LinkedEligibleRoleAssignmentId = "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}

New-MgPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params

```