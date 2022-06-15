---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0b9f80acd5e4513f5aa750f68b1273f2b4ff2e8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098740"
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
application := msgraphsdk.NewIdentity()
identity.SetApplication(application)
displayName := "Calling Bot"
application.SetDisplayName(&displayName)
id := "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
application.SetId(&id)
application.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.identity",
}
identity.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.identitySet",
}
source.SetRegion(nil)
source.SetLanguageId(nil)
source.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.participantInfo",
}
requestBody.SetTargets( []InvitationParticipantInfo {
    msgraphsdk.NewInvitationParticipantInfo(),
identity := msgraphsdk.NewIdentitySet()
    SetIdentity(identity)
user := msgraphsdk.NewIdentity()
    identity.SetUser(user)
displayName := "John"
    user.SetDisplayName(&displayName)
id := "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
    user.SetId(&id)
    user.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.identity",
    }
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
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.call",
}
result, err := graphClient.Communications().Calls().Post(requestBody)


```