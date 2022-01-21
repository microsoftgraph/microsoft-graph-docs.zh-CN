---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf0f9b8a3c438317e04b28d1c62116b3447157a2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098408"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Action = "SelfActivate"
    PrincipalId = "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f"
    RoleDefinitionId = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3"
    DirectoryScopeId = "/"
    Justification = "Need to update app roles for selected apps."
    ScheduleInfo = @{
        StartDateTime = [System.DateTime]::Parse("2021-08-17T17:40:00.000Z")
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