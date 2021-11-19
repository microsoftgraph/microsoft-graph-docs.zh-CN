---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f03a914676a0b07de7be81106429b568dcb71554
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093382"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleManagementPolicyRule()
target := msgraphsdk.NewUnifiedRoleManagementPolicyRuleTarget()
requestBody.SetTarget(target)
target.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
}
options := &msgraphsdk.UnifiedRoleManagementPolicyRuleRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
unifiedRoleManagementPolicyRuleId := "unifiedRoleManagementPolicyRule-id"
graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).RulesById(&unifiedRoleManagementPolicyRuleId).Patch(options)


```