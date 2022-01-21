---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2ffc18fcc7059e159abe1e7d07e12bac0c078e6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134408"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    "@odata.type" = "#microsoft.graph.unifiedRoleAssignment"
    RoleDefinitionId = "fe930be7-5e62-47db-91af-98c3a49a38b1"
    PrincipalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"
    DirectoryScopeId = "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
}

New-MgRoleManagementDirectoryRoleAssignment -BodyParameter $params

```