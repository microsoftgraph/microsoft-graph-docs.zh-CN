---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 994942650f1ba0e02c608d23629e7afc6be4eb86
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098813"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantAppManagementPolicy()
isEnabled := true
requestBody.SetIsEnabled(&isEnabled)
applicationRestrictions := msgraphsdk.NewAppManagementConfiguration()
requestBody.SetApplicationRestrictions(applicationRestrictions)
applicationRestrictions.SetPasswordCredentials( []PasswordCredentialConfiguration {
    msgraphsdk.NewPasswordCredentialConfiguration(),
restrictionType := "passwordAddition"
    SetRestrictionType(&restrictionType)
    SetMaxLifetime(nil)
restrictForAppsCreatedAfterDateTime, err := time.Parse(time.RFC3339, "2021-01-01T10:37:00Z")
    SetRestrictForAppsCreatedAfterDateTime(&restrictForAppsCreatedAfterDateTime)
    msgraphsdk.NewPasswordCredentialConfiguration(),
restrictionType := "passwordLifetime"
    SetRestrictionType(&restrictionType)
maxLifetime := "P4DT12H30M5S"
    SetMaxLifetime(&maxLifetime)
restrictForAppsCreatedAfterDateTime, err := time.Parse(time.RFC3339, "2017-01-01T10:37:00Z")
    SetRestrictForAppsCreatedAfterDateTime(&restrictForAppsCreatedAfterDateTime)
    msgraphsdk.NewPasswordCredentialConfiguration(),
restrictionType := "symmetricKeyAddition"
    SetRestrictionType(&restrictionType)
    SetMaxLifetime(nil)
restrictForAppsCreatedAfterDateTime, err := time.Parse(time.RFC3339, "2021-01-01T10:37:00Z")
    SetRestrictForAppsCreatedAfterDateTime(&restrictForAppsCreatedAfterDateTime)
    msgraphsdk.NewPasswordCredentialConfiguration(),
restrictionType := "customPasswordAddition"
    SetRestrictionType(&restrictionType)
    SetMaxLifetime(nil)
restrictForAppsCreatedAfterDateTime, err := time.Parse(time.RFC3339, "2015-01-01T10:37:00Z")
    SetRestrictForAppsCreatedAfterDateTime(&restrictForAppsCreatedAfterDateTime)
    msgraphsdk.NewPasswordCredentialConfiguration(),
restrictionType := "symmetricKeyLifetime"
    SetRestrictionType(&restrictionType)
maxLifetime := "P40D"
    SetMaxLifetime(&maxLifetime)
restrictForAppsCreatedAfterDateTime, err := time.Parse(time.RFC3339, "2015-01-01T10:37:00Z")
    SetRestrictForAppsCreatedAfterDateTime(&restrictForAppsCreatedAfterDateTime)
}
applicationRestrictions.SetKeyCredentials( []KeyCredentialConfiguration {
    msgraphsdk.NewKeyCredentialConfiguration(),
restrictionType := "asymmetricKeyLifetime"
    SetRestrictionType(&restrictionType)
maxLifetime := "P30D"
    SetMaxLifetime(&maxLifetime)
restrictForAppsCreatedAfterDateTime, err := time.Parse(time.RFC3339, "2015-01-01T10:37:00Z")
    SetRestrictForAppsCreatedAfterDateTime(&restrictForAppsCreatedAfterDateTime)
}
graphClient.Policies().DefaultAppManagementPolicy().Patch(requestBody)


```