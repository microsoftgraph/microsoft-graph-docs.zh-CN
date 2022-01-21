---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cf02ca0c6dc2ffdc7b06c8e1f005786dd8223f8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104029"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "Catalog One"
}

Update-MgEntitlementManagementAccessPackageCatalog -AccessPackageCatalogId $accessPackageCatalogId -BodyParameter $params

```