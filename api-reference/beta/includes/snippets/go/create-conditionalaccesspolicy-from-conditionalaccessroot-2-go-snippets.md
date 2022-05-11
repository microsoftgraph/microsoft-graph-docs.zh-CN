---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf4af52c244ed1b4e9d177e2e92db242149a5c20
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConditionalAccessPolicy()
displayName := "Block access to EXO non-trusted regions."
requestBody.SetDisplayName(&displayName)
state := "enabled"
requestBody.SetState(&state)
conditions := msgraphsdk.NewConditionalAccessConditionSet()
requestBody.SetConditions(conditions)
conditions.SetClientAppTypes( []ConditionalAccessClientApp {
    "all",
}
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
locations := msgraphsdk.NewConditionalAccessLocations()
conditions.SetLocations(locations)
locations.SetIncludeLocations( []String {
    "198ad66e-87b3-4157-85a3-8a7b51794ee9",
}
grantControls := msgraphsdk.NewConditionalAccessGrantControls()
requestBody.SetGrantControls(grantControls)
operator := "OR"
grantControls.SetOperator(&operator)
grantControls.SetBuiltInControls( []ConditionalAccessGrantControl {
    "block",
}
result, err := graphClient.Identity().ConditionalAccess().Policies().Post(requestBody)


```