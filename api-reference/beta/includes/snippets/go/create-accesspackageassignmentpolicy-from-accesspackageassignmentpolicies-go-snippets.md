---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c3a4e0e0275a128ac713c65e458908f65572afd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082845"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentPolicy()
accessPackageId := "56ff43fd-6b05-48df-9634-956a777fce6d"
requestBody.SetAccessPackageId(&accessPackageId)
displayName := "direct"
requestBody.SetDisplayName(&displayName)
description := "direct assignments by administrator"
requestBody.SetDescription(&description)
requestBody.SetAccessReviewSettings(nil)
requestorSettings := msgraphsdk.NewRequestorSettings()
requestBody.SetRequestorSettings(requestorSettings)
scopeType := "NoSubjects"
requestorSettings.SetScopeType(&scopeType)
acceptRequests := true
requestorSettings.SetAcceptRequests(&acceptRequests)
requestorSettings.SetAllowedRequestors( []UserSet {
}
requestApprovalSettings := msgraphsdk.NewApprovalSettings()
requestBody.SetRequestApprovalSettings(requestApprovalSettings)
isApprovalRequired := false
requestApprovalSettings.SetIsApprovalRequired(&isApprovalRequired)
isApprovalRequiredForExtension := false
requestApprovalSettings.SetIsApprovalRequiredForExtension(&isApprovalRequiredForExtension)
isRequestorJustificationRequired := false
requestApprovalSettings.SetIsRequestorJustificationRequired(&isRequestorJustificationRequired)
approvalMode := "NoApproval"
requestApprovalSettings.SetApprovalMode(&approvalMode)
requestApprovalSettings.SetApprovalStages( []ApprovalStage {
}
options := &msgraphsdk.AccessPackageAssignmentPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPolicies().Post(options)


```