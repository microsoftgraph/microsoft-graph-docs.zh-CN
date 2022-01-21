---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 192f4209cbc0c6b3f2065b0c1b2ec72abf142323
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093976"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    PermissionType = "delegated"
    CertifiedClientApplicationsOnly = $true
}

New-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```