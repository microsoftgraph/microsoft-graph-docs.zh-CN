---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72ddf73a9a9e09ffd9da90da5bc833a38cd8bae3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103972"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    RoleId = "roleId-value"
    RoleMemberInfo = @{
        Id = "id-value"
    }
}

New-MgAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```