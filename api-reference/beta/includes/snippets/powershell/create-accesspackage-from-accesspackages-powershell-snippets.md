---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0e657c398d9e75c0b8b53d6e850b422cdefc43e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120468"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    CatalogId = "aa2f6514-3232-46e7-a08a-2411ad8d7128"
    DisplayName = "sales reps"
    Description = "outside sales representatives"
}

New-MgEntitlementManagementAccessPackage -BodyParameter $params

```