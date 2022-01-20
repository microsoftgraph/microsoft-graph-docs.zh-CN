---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47bcf2ce78169e1e1bbf83d5f4441004ed9bd51b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134407"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    "@odata.type" = "#microsoft.graph.unifiedRoleAssignment"
    RoleDefinitionId = "c2cf284d-6c41-4e6b-afac-4b80928c9034"
    PrincipalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"
    DirectoryScopeId = "/"
}

New-MgRoleManagementDirectoryRoleAssignment -BodyParameter $params

```