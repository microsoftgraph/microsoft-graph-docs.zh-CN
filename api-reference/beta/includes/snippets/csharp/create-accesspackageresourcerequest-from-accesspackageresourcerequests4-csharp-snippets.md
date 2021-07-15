---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8a1b3d20f89ba0a8d5e019ca884dee7d907f678
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439139"
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