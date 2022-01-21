---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1861c308d380a72dcb894a3c90e3e300c230152
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134552"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId $permissionGrantPolicyId -PermissionGrantConditionSetId $permissionGrantConditionSetId

```