---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 766a36d89d997b100a0f23eebeab3fcb88ae0ae5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105142"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    PrincipalIds = @(
        "0aeec2c1-fee7-4e02-b534-6f920d25b300"
        "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"
    )
}

Update-MgRoleManagementDeviceManagementRoleAssignment -UnifiedRoleAssignmentMultipleId $unifiedRoleAssignmentMultipleId -BodyParameter $params

```