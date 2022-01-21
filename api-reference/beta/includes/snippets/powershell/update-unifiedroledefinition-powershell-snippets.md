---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e606bbb29492732e9d76be369670f75acf437f2a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089126"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Description = "Update basic properties of application registrations"
    DisplayName = "Application Registration Support Administrator"
    RolePermissions = @(
        @{
            AllowedResourceActions = @(
                "microsoft.directory/applications/basic/read"
            )
        }
    )
}

Update-MgRoleManagementDirectoryRoleDefinition -UnifiedRoleDefinitionId $unifiedRoleDefinitionId -BodyParameter $params

```