---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fef429a493ad1631a67ca1a2907c201285515ded
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329198"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentPolicy()
displayName := "New Policy"
requestBody.SetDisplayName(&displayName)
description := "policy for assignment"
requestBody.SetDescription(&description)
allowedTargetScope := "notSpecified"
requestBody.SetAllowedTargetScope(&allowedTargetScope)
requestBody.SetSpecificAllowedTargets( []SubjectSet {
}
expiration := msgraphsdk.NewExpirationPattern()
requestBody.SetExpiration(expiration)
expiration.SetEndDateTime(nil)
expiration.SetDuration(nil)
type := "noExpiration"
expiration.SetType(&type)
requestorSettings := msgraphsdk.NewAccessPackageAssignmentRequestorSettings()
requestBody.SetRequestorSettings(requestorSettings)
enableTargetsToSelfAddAccess := false
requestorSettings.SetEnableTargetsToSelfAddAccess(&enableTargetsToSelfAddAccess)
enableTargetsToSelfUpdateAccess := false
requestorSettings.SetEnableTargetsToSelfUpdateAccess(&enableTargetsToSelfUpdateAccess)
enableTargetsToSelfRemoveAccess := false
requestorSettings.SetEnableTargetsToSelfRemoveAccess(&enableTargetsToSelfRemoveAccess)
allowCustomAssignmentSchedule := true
requestorSettings.SetAllowCustomAssignmentSchedule(&allowCustomAssignmentSchedule)
enableOnBehalfRequestorsToAddAccess := false
requestorSettings.SetEnableOnBehalfRequestorsToAddAccess(&enableOnBehalfRequestorsToAddAccess)
enableOnBehalfRequestorsToUpdateAccess := false
requestorSettings.SetEnableOnBehalfRequestorsToUpdateAccess(&enableOnBehalfRequestorsToUpdateAccess)
enableOnBehalfRequestorsToRemoveAccess := false
requestorSettings.SetEnableOnBehalfRequestorsToRemoveAccess(&enableOnBehalfRequestorsToRemoveAccess)
requestorSettings.SetOnBehalfRequestors( []SubjectSet {
}
requestApprovalSettings := msgraphsdk.NewAccessPackageAssignmentApprovalSettings()
requestBody.SetRequestApprovalSettings(requestApprovalSettings)
isApprovalRequiredForAdd := false
requestApprovalSettings.SetIsApprovalRequiredForAdd(&isApprovalRequiredForAdd)
isApprovalRequiredForUpdate := false
requestApprovalSettings.SetIsApprovalRequiredForUpdate(&isApprovalRequiredForUpdate)
requestApprovalSettings.SetStages( []AccessPackageApprovalStage {
}
accessPackage := msgraphsdk.NewAccessPackage()
requestBody.SetAccessPackage(accessPackage)
id := "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
accessPackage.SetId(&id)
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentPolicies().Post(requestBody)


```