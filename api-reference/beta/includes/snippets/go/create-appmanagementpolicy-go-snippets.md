---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9fb6c704189497b3b535c580c530bd3bbe6c060
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982665"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAppManagementPolicy()
displayName := "Credential management policy"
requestBody.SetDisplayName(&displayName)
description := "Cred policy sample"
requestBody.SetDescription(&description)
isEnabled := true
requestBody.SetIsEnabled(&isEnabled)
restrictions := msgraphsdk.NewAppManagementConfiguration()
requestBody.SetRestrictions(restrictions)
restrictions.SetPasswordCredentials( []PasswordCredentialConfiguration {
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "passwordAddition",
        "maxLifetime": nil,
        "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "passwordLifetime",
        "maxLifetime": "P4DT12H30M5S",
        "restrictForAppsCreatedAfterDateTime": "2014-10-19T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "symmetricKeyAddition",
        "maxLifetime": nil,
        "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "symmetricKeyLifetime",
        "maxLifetime": "P4D",
        "restrictForAppsCreatedAfterDateTime": "2014-10-19T10:37:00Z",
    }
}
restrictions.SetKeyCredentials( []KeyCredentialConfiguration {
    msgraphsdk.NewKeyCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "asymmetricKeyLifetime",
        "maxLifetime": "P90D",
        "restrictForAppsCreatedAfterDateTime": "2014-10-19T10:37:00Z",
    }
}
options := &msgraphsdk.AppManagementPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().AppManagementPolicies().Post(options)


```