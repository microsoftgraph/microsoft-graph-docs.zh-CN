---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae93a0a3f0a907b8f4d333ad90522861c38b5e1e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439187"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Action = "adminAssign"
    Justification = "Assign Groups Admin to IT Helpdesk group"
    RoleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c"
    DirectoryScopeId = "/"
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b"
    ScheduleInfo = @{
        StartDateTime = [System.DateTime]::Parse("2022-04-10T00:00:00Z")
        Expiration = @{
            Type = "NoExpiration"
        }
    }
}

New-MgRoleManagementDirectoryRoleAssignmentScheduleRequest -BodyParameter $params

```