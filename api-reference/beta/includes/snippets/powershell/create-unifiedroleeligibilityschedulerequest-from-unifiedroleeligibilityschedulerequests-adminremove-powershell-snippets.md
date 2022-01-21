---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d7ba33ea904c55ed48fc17c67938775c3da2c2e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119853"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Action = "AdminRemove"
    Justification = "Assign User Admin eligibility to IT Helpdesk (User) group"
    RoleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c"
    DirectoryScopeId = "/"
    PrincipalId = "07706ff1-46c7-4847-ae33-3003830675a1"
    ScheduleInfo = @{
        StartDateTime = [System.DateTime]::Parse("2021-07-26T18:08:06.2081758Z")
        Expiration = @{
            EndDateTime = [System.DateTime]::Parse("2022-06-30T00:00:00Z")
            Type = "AfterDateTime"
        }
    }
}

New-MgRoleManagementDirectoryRoleEligibilityScheduleRequest -BodyParameter $params

```