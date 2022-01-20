---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c03372cb2a0112b3e001021f919615812cd8b86
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119061"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    CatalogId = "beedadfe-01d5-4025-910b-84abb9369997"
    RequestType = "AdminRemove"
    AccessPackageResource = @{
        Id = "354078e5-dbce-4894-8af4-0ab274d41662"
    }
}

New-MgEntitlementManagementAccessPackageResourceRequest -BodyParameter $params

```