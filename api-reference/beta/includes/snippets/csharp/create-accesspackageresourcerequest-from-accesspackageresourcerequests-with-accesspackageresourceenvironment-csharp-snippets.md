---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d64251bb7a1306df67a7301d3bbd119f79f6aa87f20dbe8b0895d0f6868b2f1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104166"
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
        AdditionalData = new Dictionary<string, object>()
        {
            {"accessPackageResourceEnvironment@odata.bind", "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"}
        }
    },
    RequestType = "AdminAdd"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .AddAsync(accessPackageResourceRequest);

```