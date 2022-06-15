---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 106a07cf3ab265526c5d13726e778cb4ae01ef80
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationMethodsPolicy()
registrationEnforcement := msgraphsdk.NewRegistrationEnforcement()
requestBody.SetRegistrationEnforcement(registrationEnforcement)
authenticationMethodsRegistrationCampaign := msgraphsdk.NewAuthenticationMethodsRegistrationCampaign()
registrationEnforcement.SetAuthenticationMethodsRegistrationCampaign(authenticationMethodsRegistrationCampaign)
snoozeDurationInDays := int32(1)
authenticationMethodsRegistrationCampaign.SetSnoozeDurationInDays(&snoozeDurationInDays)
state := "enabled"
authenticationMethodsRegistrationCampaign.SetState(&state)
authenticationMethodsRegistrationCampaign.SetExcludeTargets( []ExcludeTarget {
}
authenticationMethodsRegistrationCampaign.SetIncludeTargets( []AuthenticationMethodsRegistrationCampaignIncludeTarget {
    msgraphsdk.NewAuthenticationMethodsRegistrationCampaignIncludeTarget(),
    SetAdditionalData(map[string]interface{}{
        "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
        "targetType": "group",
        "targetedAuthenticationMethod": "microsoftAuthenticator",
    }
}
requestBody.SetAuthenticationMethodConfigurations( []AuthenticationMethodConfiguration {
    msgraphsdk.NewAuthenticationMethodConfiguration(),
id := "Fido2"
    SetId(&id)
state := "disabled"
    SetState(&state)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
        "isSelfServiceRegistrationAllowed": false,
        "isAttestationEnforced": false,
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy",
}
graphClient.Policies().AuthenticationMethodsPolicy().Patch(requestBody)


```