---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d2a99ebe1dbbbc4d72c84a0df31c2fd652800ef749c6113b65f140a43657a80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104218"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRoleScope = new AccessPackageResourceRoleScope
{
    AccessPackageResourceRole = new AccessPackageResourceRole
    {
        OriginId = "Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
        DisplayName = "Member",
        OriginSystem = "AadGroup",
        AccessPackageResource = new AccessPackageResource
        {
            Id = "1d08498d-72a1-403f-8511-6b1f875746a0",
            ResourceType = "O365 Group",
            OriginId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca",
            OriginSystem = "AadGroup"
        }
    },
    AccessPackageResourceScope = new AccessPackageResourceScope
    {
        OriginId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca",
        OriginSystem = "AadGroup"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].AccessPackageResourceRoleScopes
    .Request()
    .AddAsync(accessPackageResourceRoleScope);

```