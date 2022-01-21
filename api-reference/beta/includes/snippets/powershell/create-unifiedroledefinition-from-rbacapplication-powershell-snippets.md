---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a333ae3fda76a8c26bd59f0c9a15eb93cc7f5ab3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120031"
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
    IsEnabled = "true"
}

New-MgRoleManagementDirectoryRoleDefinition -BodyParameter $params

```