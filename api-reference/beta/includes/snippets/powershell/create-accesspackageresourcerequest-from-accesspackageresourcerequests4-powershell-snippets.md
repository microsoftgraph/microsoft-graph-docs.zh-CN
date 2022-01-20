---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 834f6ed29cc83ef43de98038e2ab3569c511739c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119062"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    CatalogId = "beedadfe-01d5-4025-910b-84abb9369997"
    RequestType = "AdminAdd"
    AccessPackageResource = @{
        OriginId = "c6294667-7348-4f5a-be73-9d2c65f574f3"
        OriginSystem = "AadGroup"
    }
}

New-MgEntitlementManagementAccessPackageResourceRequest -BodyParameter $params

```