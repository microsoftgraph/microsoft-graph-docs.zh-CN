---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c74f3f689c618c71292c4687af394174946401c6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098737"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCall()
callbackUri := "https://bot.contoso.com/callback"
requestBody.SetCallbackUri(&callbackUri)
source := msgraphsdk.NewParticipantInfo()
requestBody.SetSource(source)
identity := msgraphsdk.NewIdentitySet()
source.SetIdentity(identity)
identity.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.identitySet",
}
source.SetCountryCode(nil)
source.SetEndpointType(nil)
source.SetRegion(nil)
source.SetLanguageId(nil)
source.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.participantInfo",
}
requestBody.SetTargets( []InvitationParticipantInfo {
    msgraphsdk.NewInvitationParticipantInfo(),
identity := msgraphsdk.NewIdentitySet()
    SetIdentity(identity)
    identity.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.identitySet",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    }
}
requestBody.SetRequestedModalities( []Modality {
    "audio",
}
mediaConfig := msgraphsdk.NewMediaConfig()
requestBody.SetMediaConfig(mediaConfig)
mediaConfig.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
}
tenantId := "aa67bd4c-8475-432d-bd41-39f255720e0a"
requestBody.SetTenantId(&tenantId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.call",
}
result, err := graphClient.Communications().Calls().Post(requestBody)


```