---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47b8957936383d21dcff1113d08a5e4e1f619f37
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114427"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyAppManagementPolicy -AppManagementPolicyId $appManagementPolicyId

```