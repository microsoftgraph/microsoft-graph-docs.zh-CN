---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0caf8670c41d38b0b214e6dc7808b12c4b8730a795a6921bfe5743ee6b177c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158624"
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