---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e340db2f2c4cf8324aef59d34e0709334da34ebe
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412219"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
transferTarget := msgraphsdk.NewInvitationParticipantInfo()
requestBody.SetTransferTarget(transferTarget)
identity := msgraphsdk.NewIdentitySet()
transferTarget.SetIdentity(identity)
identity.SetAdditionalData(map[string]interface{}{
}
transferTarget.SetAdditionalData(map[string]interface{}{
    "endpointType": "default",
    "languageId": "languageId-value",
    "region": "region-value",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08",
}
options := &msgraphsdk.TransferRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer(call-id).Post(options)


```