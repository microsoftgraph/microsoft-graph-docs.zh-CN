---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6fe391c20e35dc595952e840543bb754eb0cb48
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983563"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessPackageAssignmentPolicy()
accessPackageId := "b2eba9a1-b357-42ee-83a8-336522ed6cbf"
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
requestApprovalSettings := msgraphsdk.NewApprovalSettings()
requestBody.SetRequestApprovalSettings(requestApprovalSettings)
isApprovalRequired := true
requestApprovalSettings.SetIsApprovalRequired(&isApprovalRequired)
isApprovalRequiredForExtension := false
requestApprovalSettings.SetIsApprovalRequiredForExtension(&isApprovalRequiredForExtension)
isRequestorJustificationRequired := true
requestApprovalSettings.SetIsRequestorJustificationRequired(&isRequestorJustificationRequired)
approvalMode := "SingleStage"
requestApprovalSettings.SetApprovalMode(&approvalMode)
requestApprovalSettings.SetApprovalStages( []ApprovalStage {
    msgraphsdk.NewApprovalStage(),
    SetAdditionalData(map[string]interface{}{
        "approvalStageTimeOutInDays": ,
        "isApproverJustificationRequired": true,
        "isEscalationEnabled": false,
        "escalationTimeInMinutes": ,
        "primaryApprovers":  []Object {
        }
    }
}
requestBody.SetQuestions( []AccessPackageQuestion {
    msgraphsdk.NewAccessPackageQuestion(),
    SetAdditionalData(map[string]interface{}{
        "isRequired": false,
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices":  []Object {
        }
        "allowsMultipleSelection": false,
    }
    msgraphsdk.NewAccessPackageQuestion(),
    SetAdditionalData(map[string]interface{}{
        "isRequired": false,
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false,
    }
}
options := &msgraphsdk.AccessPackageAssignmentPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPolicies().Post(options)


```