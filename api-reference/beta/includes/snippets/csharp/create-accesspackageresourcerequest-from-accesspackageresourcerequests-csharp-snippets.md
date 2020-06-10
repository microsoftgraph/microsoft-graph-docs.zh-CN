---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b35441e79c12e16028a9deb25c3727e626123e28
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRequest = new AccessPackageResourceRequestObject
{
    CatalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
    RequestType = "AdminAdd",
    Justification = "",
    AccessPackageResource = new AccessPackageResource
    {
        DisplayName = "Sales",
        Description = "https://contoso.sharepoint.com/sites/Sales",
        Url = "https://contoso.sharepoint.com/sites/Sales",
        ResourceType = "SharePoint Online Site",
        OriginId = "https://contoso.sharepoint.com/sites/Sales",
        OriginSystem = "SharePointOnline"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .AddAsync(accessPackageResourceRequest);

```