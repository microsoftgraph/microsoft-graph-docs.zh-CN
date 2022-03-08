---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cacbdc09bd25eb6e89f2d4c0fa8b8f75a0d51d4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335855"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicyConfigurationPartner = new CrossTenantAccessPolicyConfigurationPartner
{
    TenantId = "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a",
    B2bDirectConnectOutbound = new CrossTenantAccessPolicyB2BSetting
    {
        UsersAndGroups = new CrossTenantAccessPolicyTargetConfiguration
        {
            AccessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked,
            Targets = new List<CrossTenantAccessPolicyTarget>()
            {
                new CrossTenantAccessPolicyTarget
                {
                    Target = "6f546279-4da5-4b53-a095-09ea0cef9971",
                    TargetType = CrossTenantAccessPolicyTargetType.Group
                }
            }
        }
    },
    B2bDirectConnectInbound = new CrossTenantAccessPolicyB2BSetting
    {
        Applications = new CrossTenantAccessPolicyTargetConfiguration
        {
            AccessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Allowed,
            Targets = new List<CrossTenantAccessPolicyTarget>()
            {
                new CrossTenantAccessPolicyTarget
                {
                    Target = "Office365",
                    TargetType = CrossTenantAccessPolicyTargetType.Application
                }
            }
        }
    }
};

await graphClient.Policies.CrossTenantAccessPolicy.Partners
    .Request()
    .AddAsync(crossTenantAccessPolicyConfigurationPartner);

```