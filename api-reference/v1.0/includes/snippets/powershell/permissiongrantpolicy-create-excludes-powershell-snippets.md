---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd1ff9b1b68611049fee00ff4298c063754ba402
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124598"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    PermissionType = "delegated"
    ResourceApplication = "00000003-0000-0000-c000-000000000000"
}

New-MgPolicyPermissionGrantPolicyExclude -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```