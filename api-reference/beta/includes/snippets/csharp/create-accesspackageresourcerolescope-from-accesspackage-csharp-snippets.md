---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c325a3ff2a105a680987b4fb7d281b9e3f902dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796367"
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