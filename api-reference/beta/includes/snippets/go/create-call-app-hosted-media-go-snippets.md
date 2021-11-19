---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4faca41b077c219e93c2083d0f3f9e5c6b2997ce
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087496"
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
options := &msgraphsdk.CallsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Communications().Calls().Post(options)


```