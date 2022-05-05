---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 986c5ac46ee08cc95686f32ecc1f46118ca9ff91
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminAccessAssignment = new DelegatedAdminAccessAssignment
{
    AccessContainer = new DelegatedAdminAccessContainer
    {
        AccessContainerId = "869713c9-0b28-4d08-8949-ae07ae1bf528",
        AccessContainerType = DelegatedAdminAccessContainerType.SecurityGroup
    },
    AccessDetails = new DelegatedAdminAccessDetails
    {
        UnifiedRoles = new List<UnifiedRole>()
        {
            new UnifiedRole
            {
                RoleDefinitionId = "29232cdf-9323-42fd-ade2-1d097af3e4de"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "729827e3-9c14-49f7-bb1b-9608f156bbb8"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "3a2c62db-5318-420d-8d74-23affee5d9d5"
            }
        }
    }
};

await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].AccessAssignments
    .Request()
    .AddAsync(delegatedAdminAccessAssignment);

```