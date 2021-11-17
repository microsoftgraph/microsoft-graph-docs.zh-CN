---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70ac1fb2aa97c2e0c5aed28d0ea7acf4aab75fc3bc1a952ee523b32a756c05bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRequest = new AccessPackageResourceRequestObject
{
    CatalogId = "de9315c1-272b-4905-924b-cc112ca180c7",
    AccessPackageResource = new AccessPackageResource
    {
        DisplayName = "Community Outreach",
        Description = "https://contoso.sharepoint.com/sites/CSR",
        ResourceType = "SharePoint Online Site",
        OriginId = "https://contoso.sharepoint.com/sites/CSR",
        OriginSystem = "SharePointOnline",
        AccessPackageResourceEnvironment = new AccessPackageResourceEnvironment
        {
            OriginId = "https://contoso-admin.sharepoint.com/"
        }
    },
    RequestType = "AdminAdd"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .AddAsync(accessPackageResourceRequest);

```