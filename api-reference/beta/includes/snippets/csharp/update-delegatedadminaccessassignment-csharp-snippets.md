---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc48538526c4e169b93173246d7c399e8c11e8b1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminAccessAssignment = new DelegatedAdminAccessAssignment
{
    AccessDetails = new DelegatedAdminAccessDetails
    {
        UnifiedRoles = new List<UnifiedRole>()
        {
            new UnifiedRole
            {
                RoleDefinitionId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "44367163-eba1-44c3-98af-f5787879f96a"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "729827e3-9c14-49f7-bb1b-9608f156bbb8"
            }
        }
    }
};

await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].AccessAssignments["{delegatedAdminAccessAssignment-id}"]
    .Request()
    .Header("If-Match","W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"")
    .UpdateAsync(delegatedAdminAccessAssignment);

```