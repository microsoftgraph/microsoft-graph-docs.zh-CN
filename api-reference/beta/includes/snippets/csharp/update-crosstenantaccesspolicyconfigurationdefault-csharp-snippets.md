---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 328c8c94229bd2b424d2b9f55200e1d4b93e2b49
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicyConfigurationDefault = new CrossTenantAccessPolicyConfigurationDefault
{
    B2bCollaborationOutbound = new CrossTenantAccessPolicyB2BSetting
    {
        UsersAndGroups = new CrossTenantAccessPolicyTargetConfiguration
        {
            AccessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked,
            Targets = new List<CrossTenantAccessPolicyTarget>()
            {
                new CrossTenantAccessPolicyTarget
                {
                    Target = "0be493dc-cb56-4a53-936f-9cf64410b8b0",
                    TargetType = CrossTenantAccessPolicyTargetType.Group
                }
            }
        },
        Applications = new CrossTenantAccessPolicyTargetConfiguration
        {
            AccessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked,
            Targets = new List<CrossTenantAccessPolicyTarget>()
            {
                new CrossTenantAccessPolicyTarget
                {
                    Target = "AllApplications",
                    TargetType = CrossTenantAccessPolicyTargetType.Application
                }
            }
        }
    }
};

await graphClient.Policies.CrossTenantAccessPolicy.Default
    .Request()
    .UpdateAsync(crossTenantAccessPolicyConfigurationDefault);

```