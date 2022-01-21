---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4ff0408deb25f6dca9cfdfaf0200648691a79fc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088879"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    RoleId = "roleId-value"
    RoleMemberInfo = @{
        Id = "id-value"
    }
}

New-MgDirectoryAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```