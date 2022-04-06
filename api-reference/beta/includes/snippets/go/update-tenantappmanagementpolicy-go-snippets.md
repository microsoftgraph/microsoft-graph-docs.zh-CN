---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a791aa14025cb4a32f45cb9a96147685f2a29fac
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528153"
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
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "passwordAddition",
        "maxLifetime": nil,
        "restrictForAppsCreatedAfterDateTime": "2021-01-01T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "passwordLifetime",
        "maxLifetime": "P4DT12H30M5S",
        "restrictForAppsCreatedAfterDateTime": "2017-01-01T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "symmetricKeyAddition",
        "maxLifetime": nil,
        "restrictForAppsCreatedAfterDateTime": "2021-01-01T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "customPasswordAddition",
        "maxLifetime": nil,
        "restrictForAppsCreatedAfterDateTime": "2015-01-01T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "symmetricKeyLifetime",
        "maxLifetime": "P40D",
        "restrictForAppsCreatedAfterDateTime": "2015-01-01T10:37:00Z",
    }
}
applicationRestrictions.SetKeyCredentials( []KeyCredentialConfiguration {
    msgraphsdk.NewKeyCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "asymmetricKeyLifetime",
        "maxLifetime": "P30D",
        "restrictForAppsCreatedAfterDateTime": "2015-01-01T10:37:00Z",
    }
}
options := &msgraphsdk.DefaultAppManagementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().DefaultAppManagementPolicy().Patch(options)


```