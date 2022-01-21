---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f290a3a61ddd38e7335d94d93cd8cf0755c70a9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125691"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    PrincipalId = "679a9213-c497-48a4-830a-8d3d25d94ddc"
    RoleDefinitionId = "ae79f266-94d4-4dab-b730-feca7e132178"
    AppScopeId = "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}

New-MgRoleManagementEntitlementManagementRoleAssignment -BodyParameter $params

```