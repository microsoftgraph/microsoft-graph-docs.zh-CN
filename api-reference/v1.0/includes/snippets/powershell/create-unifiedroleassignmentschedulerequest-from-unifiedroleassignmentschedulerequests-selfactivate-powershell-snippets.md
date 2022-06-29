---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 667b3fffc8dfc94c88d8537bc1a6e0e084d0fd06
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439188"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Action = "selfActivate"
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b"
    RoleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4"
    DirectoryScopeId = "/"
    Justification = "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs"
    ScheduleInfo = @{
        StartDateTime = [System.DateTime]::Parse("2022-04-14T00:00:00.000Z")
        Expiration = @{
            Type = "AfterDuration"
            Duration = "PT5H"
        }
    }
    TicketInfo = @{
        TicketNumber = "CONTOSO:Normal-67890"
        TicketSystem = "MS Project"
    }
}

New-MgRoleManagementDirectoryRoleAssignmentScheduleRequest -BodyParameter $params

```