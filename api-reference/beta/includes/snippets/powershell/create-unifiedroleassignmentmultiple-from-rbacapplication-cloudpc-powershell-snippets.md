---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f09dd26297ff42fac6f9e9c17747e46117115b0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135145"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    "@odata.type" = "#microsoft.graph.unifiedRoleAssignmentMultiple"
    DisplayName = "My test role assignment 1"
    Description = "My role assignment description"
    RoleDefinitionId = "b5c08161-a7af-481c-ace2-a20a69a48fb1"
    PrincipalIds = @(
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"
        "c1518aa9-4da5-4c84-a902-a31404023890"
    )
}

New-MgRoleManagementCloudPcRoleAssignment -BodyParameter $params

```