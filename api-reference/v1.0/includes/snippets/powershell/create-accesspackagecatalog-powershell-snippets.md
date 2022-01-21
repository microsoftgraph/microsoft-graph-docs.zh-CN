---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c59ce52d8490658dab4f7e6ca89e87c4e95b181e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114980"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "sales"
    Description = "for employees working with sales and outside sales partners"
    State = "published"
    IsExternallyVisible = $true
}

New-MgEntitlementManagementCatalog -BodyParameter $params

```