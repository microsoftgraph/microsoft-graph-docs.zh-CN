---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0525d805b7889ac96c83d752d39659ce31207809
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094142"
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
user := msgraphsdk.NewIdentity()
identity.SetUser(user)
id := "550fae72-d251-43ec-868c-373732c2704f"
user.SetId(&id)
displayName := "Heidi Steen"
user.SetDisplayName(&displayName)
user.SetAdditionalData(map[string]interface{}{
    "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
}
transferTarget.SetAdditionalData(map[string]interface{}{
    "languageId": "languageId-value",
    "region": "region-value",
}
options := &msgraphsdk.TransferRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer().Post(options)


```