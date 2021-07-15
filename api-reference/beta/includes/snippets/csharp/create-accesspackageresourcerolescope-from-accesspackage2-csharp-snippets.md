---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: debc38c505b3933c1ba2b8cf9bb24b894510dc99
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439878"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRoleScope = new AccessPackageResourceRoleScope
{
    AccessPackageResourceRole = new AccessPackageResourceRole
    {
        OriginId = "4",
        OriginSystem = "SharePointOnline",
        AccessPackageResource = new AccessPackageResource
        {
            Id = "53c71803-a0a8-4777-aecc-075de8ee3991"
        }
    },
    AccessPackageResourceScope = new AccessPackageResourceScope
    {
        Id = "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33",
        OriginId = "https://microsoft.sharepoint.com/portals/Community",
        OriginSystem = "SharePointOnline"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].AccessPackageResourceRoleScopes
    .Request()
    .AddAsync(accessPackageResourceRoleScope);

```