---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a413769a3bd739402866cc8db57a01278af1277
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220336"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule"
    Id = "Expiration_EndUser_Assignment"
    IsExpirationRequired = $true
    MaximumDuration = "PT1H45M"
    Target = @{
        "@odata.type" = "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
        Caller = "EndUser"
        Operations = @(
            "All"
        )
        Level = "Assignment"
        InheritableSettings = @(
        )
        EnforcedSettings = @(
        )
    }
}

Update-MgPolicyRoleManagementPolicyRule -UnifiedRoleManagementPolicyId $unifiedRoleManagementPolicyId -UnifiedRoleManagementPolicyRuleId $unifiedRoleManagementPolicyRuleId -BodyParameter $params

```