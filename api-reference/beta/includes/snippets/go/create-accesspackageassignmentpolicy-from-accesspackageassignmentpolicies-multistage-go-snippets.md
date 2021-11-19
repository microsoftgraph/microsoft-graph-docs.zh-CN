---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b74b9854c29801bb202fb7f63bb4b990c371cad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082847"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentPolicy()
accessPackageId := "string (identifier)"
requestBody.SetAccessPackageId(&accessPackageId)
displayName := "Users from connected organizations can request"
requestBody.SetDisplayName(&displayName)
description := "Allow users from configured connected organizations to request and be approved by their sponsors"
requestBody.SetDescription(&description)
canExtend := false
requestBody.SetCanExtend(&canExtend)
durationInDays := int32(365)
requestBody.SetDurationInDays(&durationInDays)
requestBody.SetExpirationDateTime(nil)
requestorSettings := msgraphsdk.NewRequestorSettings()
requestBody.SetRequestorSettings(requestorSettings)
scopeType := "AllExistingConnectedOrganizationSubjects"
requestorSettings.SetScopeType(&scopeType)
acceptRequests := true
requestorSettings.SetAcceptRequests(&acceptRequests)
requestorSettings.SetAllowedRequestors( []UserSet {
}
requestApprovalSettings := msgraphsdk.NewApprovalSettings()
requestBody.SetRequestApprovalSettings(requestApprovalSettings)
isApprovalRequired := true
requestApprovalSettings.SetIsApprovalRequired(&isApprovalRequired)
isApprovalRequiredForExtension := false
requestApprovalSettings.SetIsApprovalRequiredForExtension(&isApprovalRequiredForExtension)
isRequestorJustificationRequired := true
requestApprovalSettings.SetIsRequestorJustificationRequired(&isRequestorJustificationRequired)
approvalMode := "Serial"
requestApprovalSettings.SetApprovalMode(&approvalMode)
requestApprovalSettings.SetApprovalStages( []ApprovalStage {
    msgraphsdk.NewApprovalStage(),
    SetAdditionalData(map[string]interface{}{
        "approvalStageTimeOutInDays": ,
        "isApproverJustificationRequired": true,
        "isEscalationEnabled": true,
        "escalationTimeInMinutes": ,
        "primaryApprovers":  []Object {
        }
        "escalationApprovers":  []Object {
        }
    }
    msgraphsdk.NewApprovalStage(),
    SetAdditionalData(map[string]interface{}{
        "approvalStageTimeOutInDays": ,
        "isApproverJustificationRequired": true,
        "isEscalationEnabled": true,
        "escalationTimeInMinutes": ,
        "primaryApprovers":  []Object {
        }
        "escalationApprovers":  []Object {
        }
    }
}
accessReviewSettings := msgraphsdk.NewAssignmentReviewSettings()
requestBody.SetAccessReviewSettings(accessReviewSettings)
isEnabled := true
accessReviewSettings.SetIsEnabled(&isEnabled)
recurrenceType := "quarterly"
accessReviewSettings.SetRecurrenceType(&recurrenceType)
reviewerType := "Self"
accessReviewSettings.SetReviewerType(&reviewerType)
startDateTime, err := time.Parse(time.RFC3339, "2020-04-01T07:59:59.998Z")
accessReviewSettings.SetStartDateTime(&startDateTime)
durationInDays := int32(25)
accessReviewSettings.SetDurationInDays(&durationInDays)
accessReviewSettings.SetReviewers( []UserSet {
}
options := &msgraphsdk.AccessPackageAssignmentPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPolicies().Post(options)


```