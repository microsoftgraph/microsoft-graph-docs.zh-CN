---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bf07bcd0d759f437278c3ec32c6ea4b389de37a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminRelationship = new DelegatedAdminRelationship
{
    DisplayName = "Updated Contoso admin relationship",
    Duration = new Duration("P31D"),
    Customer = new DelegatedAdminRelationshipCustomerParticipant
    {
        TenantId = "52eaad04-13a2-4a2f-9ce8-93a294fadf36"
    },
    AccessDetails = new DelegatedAdminAccessDetails
    {
        UnifiedRoles = new List<UnifiedRole>()
        {
            new UnifiedRole
            {
                RoleDefinitionId = "44367163-eba1-44c3-98af-f5787879f96a"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "29232cdf-9323-42fd-ade2-1d097af3e4de"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "69091246-20e8-4a56-aa4d-066075b2a7a8"
            },
            new UnifiedRole
            {
                RoleDefinitionId = "3a2c62db-5318-420d-8d74-23affee5d9d5"
            }
        }
    }
};

await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"]
    .Request()
    .Header("If-Match","W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"")
    .UpdateAsync(delegatedAdminRelationship);

```