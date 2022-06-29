---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcc8ac9eeee5c6df646489d065185caa129cce2d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439851"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Action = "adminAssign"
    Justification = "Assign Attribute Assignment Admin eligibility to restricted user"
    RoleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4"
    DirectoryScopeId = "/"
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b"
    ScheduleInfo = @{
        StartDateTime = [System.DateTime]::Parse("2022-04-10T00:00:00Z")
        Expiration = @{
            Type = "afterDateTime"
            EndDateTime = [System.DateTime]::Parse("2024-04-10T00:00:00Z")
        }
    }
}

New-MgRoleManagementDirectoryRoleEligibilityScheduleRequest -BodyParameter $params

```