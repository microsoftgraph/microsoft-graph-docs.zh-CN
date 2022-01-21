---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e05d01eaab4851adff50b57a253df3fa27319f4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119065"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    CatalogId = "de9315c1-272b-4905-924b-cc112ca180c7"
    AccessPackageResource = @{
        DisplayName = "Community Outreach"
        Description = "https://contoso.sharepoint.com/sites/CSR"
        ResourceType = "SharePoint Online Site"
        OriginId = "https://contoso.sharepoint.com/sites/CSR"
        OriginSystem = "SharePointOnline"
        "AccessPackageResourceEnvironment@odata.bind" = "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"
    }
    RequestType = "AdminAdd"
}

New-MgEntitlementManagementAccessPackageResourceRequest -BodyParameter $params

```