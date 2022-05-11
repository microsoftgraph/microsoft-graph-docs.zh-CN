---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1275ce6c3751a3da0180c952fa4dd5277cb3b686
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327034"
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
callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer(call-id).Post(requestBody)


```