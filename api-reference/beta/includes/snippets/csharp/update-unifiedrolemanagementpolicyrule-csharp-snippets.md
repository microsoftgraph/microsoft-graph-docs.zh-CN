---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba7c33ac23f9531c40439c0c8aff7cb9a2ef0648
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474263"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicyRule = new UnifiedRoleManagementPolicyRule
{
    Target = new UnifiedRoleManagementPolicyRuleTarget
    {
    }
};

await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].Rules["{unifiedRoleManagementPolicyRule-id}"]
    .Request()
    .UpdateAsync(unifiedRoleManagementPolicyRule);

```