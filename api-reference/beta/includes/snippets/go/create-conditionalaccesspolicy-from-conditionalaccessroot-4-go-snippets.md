---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dc9823784b18f57ef2b358b81aec81177cd9388
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005791"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConditionalAccessPolicy()
displayName := "Require MFA to EXO from non-complaint devices."
requestBody.SetDisplayName(&displayName)
state := "enabled"
requestBody.SetState(&state)
conditions := msgraphsdk.NewConditionalAccessConditionSet()
requestBody.SetConditions(conditions)
applications := msgraphsdk.NewConditionalAccessApplications()
conditions.SetApplications(applications)
applications.SetIncludeApplications( []String {
    "00000002-0000-0ff1-ce00-000000000000",
}
users := msgraphsdk.NewConditionalAccessUsers()
conditions.SetUsers(users)
users.SetIncludeGroups( []String {
    "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba",
}
devices := msgraphsdk.NewConditionalAccessDevices()
conditions.SetDevices(devices)
devices.SetIncludeDevices( []String {
    "All",
}
devices.SetExcludeDevices( []String {
    "Compliant",
}
grantControls := msgraphsdk.NewConditionalAccessGrantControls()
requestBody.SetGrantControls(grantControls)
operator := "OR"
grantControls.SetOperator(&operator)
grantControls.SetBuiltInControls( []ConditionalAccessGrantControl {
    "mfa",
}
options := &msgraphsdk.PoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().ConditionalAccess().Policies().Post(options)


```