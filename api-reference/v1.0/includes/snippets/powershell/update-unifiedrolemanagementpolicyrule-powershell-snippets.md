---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a413769a3bd739402866cc8db57a01278af1277
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439753"
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