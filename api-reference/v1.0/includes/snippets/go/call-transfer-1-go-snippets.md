---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8b700dcb0b33badddae9c30d7a886e68c4dd501
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412218"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
transferTarget := msgraphsdk.NewInvitationParticipantInfo()
requestBody.SetTransferTarget(transferTarget)
identity := msgraphsdk.NewIdentitySet()
transferTarget.SetIdentity(identity)
user := msgraphsdk.NewIdentity()
identity.SetUser(user)
id := "550fae72-d251-43ec-868c-373732c2704f"
user.SetId(&id)
displayName := "Heidi Steen"
user.SetDisplayName(&displayName)
transferTarget.SetAdditionalData(map[string]interface{}{
    "endpointType": "default",
}
options := &msgraphsdk.TransferRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer(call-id).Post(options)


```