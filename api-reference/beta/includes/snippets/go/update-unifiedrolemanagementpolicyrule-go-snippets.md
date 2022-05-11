---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b2dae0c151f150602324841ae570131207d2e6a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329119"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleManagementPolicyRule()
id := "Expiration_EndUser_Assignment"
requestBody.SetId(&id)
target := msgraphsdk.NewUnifiedRoleManagementPolicyRuleTarget()
requestBody.SetTarget(target)
caller := "EndUser"
target.SetCaller(&caller)
target.SetOperations( []String {
    "All",
}
level := "Assignment"
target.SetLevel(&level)
target.SetInheritableSettings( []string {
}
target.SetEnforcedSettings( []string {
}
target.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
    "isExpirationRequired": true,
    "maximumDuration": "PT1H45M",
}
unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
unifiedRoleManagementPolicyRuleId := "unifiedRoleManagementPolicyRule-id"
graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).RulesById(&unifiedRoleManagementPolicyRuleId).Patch(requestBody)


```