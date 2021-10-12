---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12ce696b267e62c018ab6d9545a2e026f83bb739bae58890cecdf9f090a77794
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104215"
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