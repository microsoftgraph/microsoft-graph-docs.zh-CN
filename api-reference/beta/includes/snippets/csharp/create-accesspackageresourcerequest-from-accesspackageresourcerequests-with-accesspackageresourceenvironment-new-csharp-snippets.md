---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65b27cd7077a316a07bf4f7ad0caa3b9bba8fcbb
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176343"
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