---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eade1616fc167d41acf1b48ca497e5880d97315b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminRelationship = new DelegatedAdminRelationship
{
    DisplayName = "Contoso admin relationship",
    Duration = new Duration("P730D"),
    Customer = new DelegatedAdminRelationshipCustomerParticipant
    {
        TenantId = "4b827261-d21f-4aa9-b7db-7fa1f56fb163",
        DisplayName = "Contoso subsidiary Inc"
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
                RoleDefinitionId = "3a2c62db-5318-420d-8d74-23affee5d9d5"
            }
        }
    }
};

await graphClient.TenantRelationships.DelegatedAdminRelationships
    .Request()
    .AddAsync(delegatedAdminRelationship);

```