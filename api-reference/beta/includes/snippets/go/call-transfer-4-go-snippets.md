---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52fb606e1cf4d872cc57756b3df14a83a0057ca2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411695"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
transferTarget := msgraphsdk.NewInvitationParticipantInfo()
requestBody.SetTransferTarget(transferTarget)
endpointType := "default"
transferTarget.SetEndpointType(&endpointType)
identity := msgraphsdk.NewIdentitySet()
transferTarget.SetIdentity(identity)
identity.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.identitySet",
}
replacesCallId := "e5d39592-99bd-4db8-bca8-30fb894ec51d"
transferTarget.SetReplacesCallId(&replacesCallId)
transferTarget.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    "languageId": "en-us",
    "region": "amer",
}
options := &msgraphsdk.TransferRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer(call-id).Post(options)


```