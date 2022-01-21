---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9946000e122782f5878f4b793b93d0b7bbecec5e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135945"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "Custom permission grant policy"
}

Update-MgPolicyPermissionGrantPolicy -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```