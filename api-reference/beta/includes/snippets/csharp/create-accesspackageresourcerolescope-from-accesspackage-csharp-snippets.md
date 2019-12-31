---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd8db9bb0939fadc6b285cf475380de34dcef0d2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911568"
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

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{id}"].AccessPackageResourceRoleScopes
    .Request()
    .AddAsync(accessPackageResourceRoleScope);

```