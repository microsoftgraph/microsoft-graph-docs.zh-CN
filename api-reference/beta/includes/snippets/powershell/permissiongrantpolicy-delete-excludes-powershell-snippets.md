---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b94470971b1ad810c7f189298429109e8a6d6ba
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137107"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyPermissionGrantPolicyExclude -PermissionGrantPolicyId $permissionGrantPolicyId -PermissionGrantConditionSetId $permissionGrantConditionSetId

```