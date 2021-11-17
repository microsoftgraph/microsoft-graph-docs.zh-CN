---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ea78a638f99d39c93504a3b852e3b6dbf665a49
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006947"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.Communications().CallsById(&callId).Transfer().Post(options)


```