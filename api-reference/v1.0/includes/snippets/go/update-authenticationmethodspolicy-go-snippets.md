---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 809d5d454c70912be809e1ce7f867483972c50f0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093878"
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
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
        "id": "Fido2",
        "state": "disabled",
        "isSelfServiceRegistrationAllowed": false,
        "isAttestationEnforced": false,
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy",
}
options := &msgraphsdk.AuthenticationMethodsPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().AuthenticationMethodsPolicy().Patch(options)


```