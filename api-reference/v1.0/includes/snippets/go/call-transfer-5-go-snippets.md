---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e41bac5f3141eb996f6092d37c82221c1d288855
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325750"
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
transferee := msgraphsdk.NewParticipantInfo()
requestBody.SetTransferee(transferee)
identity := msgraphsdk.NewIdentitySet()
transferee.SetIdentity(identity)
user := msgraphsdk.NewIdentity()
identity.SetUser(user)
id := "751f6800-3180-414d-bd94-333364659951"
user.SetId(&id)
user.SetAdditionalData(map[string]interface{}{
    "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
}
participantId := "909c6581-5130-43e9-88f3-fcb3582cde37"
transferee.SetParticipantId(&participantId)
callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer(call-id).Post(requestBody)


```