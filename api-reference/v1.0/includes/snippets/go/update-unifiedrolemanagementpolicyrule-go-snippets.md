---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 317fea08f906739083069e277e422fb5c36c3635
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204418"
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
target.SetOperations( []UnifiedRoleManagementPolicyRuleTargetOperations {
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
options := &msgraphsdk.UnifiedRoleManagementPolicyRuleRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
unifiedRoleManagementPolicyRuleId := "unifiedRoleManagementPolicyRule-id"
graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).RulesById(&unifiedRoleManagementPolicyRuleId).Patch(options)


```