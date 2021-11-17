---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1fbc09b41a832a7eee7654eca8bb86953d3be4dcdc6d64464772f0209721e4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902748"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRequest = new AccessPackageResourceRequestObject
{
    CatalogId = "beedadfe-01d5-4025-910b-84abb9369997",
    RequestType = "AdminAdd",
    AccessPackageResource = new AccessPackageResource
    {
        OriginId = "c6294667-7348-4f5a-be73-9d2c65f574f3",
        OriginSystem = "AadGroup"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .AddAsync(accessPackageResourceRequest);

```