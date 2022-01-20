---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 270e3bac0c8161b82f996d88d61d120878698abe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097494"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    AccessPackageResourceRole = @{
        OriginId = "Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca"
        DisplayName = "Member"
        OriginSystem = "AadGroup"
        AccessPackageResource = @{
            Id = "1d08498d-72a1-403f-8511-6b1f875746a0"
            ResourceType = "O365 Group"
            OriginId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca"
            OriginSystem = "AadGroup"
        }
    }
    AccessPackageResourceScope = @{
        OriginId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca"
        OriginSystem = "AadGroup"
    }
}

New-MgEntitlementManagementAccessPackageResourceRoleScope -AccessPackageId $accessPackageId -BodyParameter $params

```