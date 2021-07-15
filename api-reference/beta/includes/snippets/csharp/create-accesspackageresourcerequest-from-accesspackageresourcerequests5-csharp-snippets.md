---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e9302e4bbe47528b03302dbed07bfe0d745cffe
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439138"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRequest = new AccessPackageResourceRequestObject
{
    CatalogId = "beedadfe-01d5-4025-910b-84abb9369997",
    RequestType = "AdminRemove",
    AccessPackageResource = new AccessPackageResource
    {
        Id = "354078e5-dbce-4894-8af4-0ab274d41662"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .AddAsync(accessPackageResourceRequest);

```