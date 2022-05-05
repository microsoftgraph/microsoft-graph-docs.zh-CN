---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1abc24b2f0d70157ee169b093311beeab18d561
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicyRule = new UnifiedRoleManagementPolicyExpirationRule
{
    Id = "Expiration_EndUser_Assignment",
    IsExpirationRequired = true,
    MaximumDuration = new Duration("PT1H45M"),
    Target = new UnifiedRoleManagementPolicyRuleTarget
    {
        Caller = "EndUser",
        Operations = new List<UnifiedRoleManagementPolicyRuleTargetOperations>()
        {
            UnifiedRoleManagementPolicyRuleTargetOperations.All
        },
        Level = "Assignment",
        InheritableSettings = new List<String>()
        {
        },
        EnforcedSettings = new List<String>()
        {
        }
    }
};

await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].Rules["{unifiedRoleManagementPolicyRule-id}"]
    .Request()
    .UpdateAsync(unifiedRoleManagementPolicyRule);

```