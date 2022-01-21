---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e58aee4879902770a95950e7352730e5c323555a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129851"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RequestType = "AdminAdd"
    AccessPackageAssignment = @{
        Target = @{
            Email = "user@contoso.com"
        }
        AssignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8"
        AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b"
    }
}

New-MgEntitlementManagementAccessPackageAssignmentRequest -BodyParameter $params

```