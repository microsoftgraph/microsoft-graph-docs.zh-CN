---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e55e287990704eafbb0bed093a4cc62c2197dcd5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119063"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    CatalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5"
    RequestType = "AdminAdd"
    Justification = ""
    AccessPackageResource = @{
        DisplayName = "Sales"
        Description = "https://contoso.sharepoint.com/sites/Sales"
        Url = "https://contoso.sharepoint.com/sites/Sales"
        ResourceType = "SharePoint Online Site"
        OriginId = "https://contoso.sharepoint.com/sites/Sales"
        OriginSystem = "SharePointOnline"
    }
}

New-MgEntitlementManagementAccessPackageResourceRequest -BodyParameter $params

```