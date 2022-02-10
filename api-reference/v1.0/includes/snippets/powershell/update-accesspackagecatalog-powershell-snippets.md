---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9d4b1325ed94666203e968d8c65de9b48cf73e6
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519615"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "Catalog One"
}

Update-MgEntitlementManagementCatalog -AccessPackageCatalogId $accessPackageCatalogId -BodyParameter $params

```