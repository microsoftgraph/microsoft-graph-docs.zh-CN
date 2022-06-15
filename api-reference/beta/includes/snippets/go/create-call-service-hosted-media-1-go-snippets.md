---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80982e9be36905a3664ee7acf54c775101c602aa
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098658"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCall()
callbackUri := "https://bot.contoso.com/callback"
requestBody.SetCallbackUri(&callbackUri)
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
callOptions := msgraphsdk.NewCallOptions()
requestBody.SetCallOptions(callOptions)
isContentSharingNotificationEnabled := true
callOptions.SetIsContentSharingNotificationEnabled(&isContentSharingNotificationEnabled)
callOptions.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.outgoingCallOptions",
}
mediaConfig := msgraphsdk.NewMediaConfig()
requestBody.SetMediaConfig(mediaConfig)
mediaConfig.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.call",
}
result, err := graphClient.Communications().Calls().Post(requestBody)


```