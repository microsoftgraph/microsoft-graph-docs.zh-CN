---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 630fe51219e5b52023775cf324ecc0528520bf62
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327082"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConditionalAccessPolicy()
displayName := "Access to EXO requires MFA"
requestBody.SetDisplayName(&displayName)
state := "enabled"
requestBody.SetState(&state)
conditions := msgraphsdk.NewConditionalAccessConditionSet()
requestBody.SetConditions(conditions)
conditions.SetClientAppTypes( []ConditionalAccessClientApp {
    "mobileAppsAndDesktopClients",
    "browser",
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
    "All",
}
locations.SetExcludeLocations( []String {
    "AllTrusted",
}
grantControls := msgraphsdk.NewConditionalAccessGrantControls()
requestBody.SetGrantControls(grantControls)
operator := "OR"
grantControls.SetOperator(&operator)
grantControls.SetBuiltInControls( []ConditionalAccessGrantControl {
    "mfa",
}
result, err := graphClient.Identity().ConditionalAccess().Policies().Post(requestBody)


```