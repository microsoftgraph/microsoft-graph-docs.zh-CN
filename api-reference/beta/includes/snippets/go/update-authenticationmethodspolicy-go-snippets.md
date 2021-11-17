---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c75f5a4ea0ef918a16a27a59cbebe2ea28ef7a17
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000019"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.AuthenticationMethodsPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().AuthenticationMethodsPolicy().Patch(options)


```