---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d73b5c6e64eb06e9afe062a1c5c97a52041e36ab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006945"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.Communications().CallsById(&callId).Transfer().Post(options)


```