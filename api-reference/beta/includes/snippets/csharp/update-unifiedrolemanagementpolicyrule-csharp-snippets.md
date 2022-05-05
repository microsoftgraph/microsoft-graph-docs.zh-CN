---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0ad3382729b3d779d26b75f9ca49f3f6be26a20
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220333"
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
        Operations = new List<String>()
        {
            "All"
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