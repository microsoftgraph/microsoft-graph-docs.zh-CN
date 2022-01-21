---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e5d7e57616ea4a686a75fd81511ee03bd0bb261
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135146"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    "@odata.type" = "#microsoft.graph.unifiedRoleAssignmentMultiple"
    DisplayName = "My test role assignment 1"
    RoleDefinitionId = "c2cf284d-6c41-4e6b-afac-4b80928c9034"
    PrincipalIds = @(
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"
        "c1518aa9-4da5-4c84-a902-a31404023890"
    )
    AppScopeIds = @(
        "allDevices"
    )
}

New-MgRoleManagementDeviceManagementRoleAssignment -BodyParameter $params

```