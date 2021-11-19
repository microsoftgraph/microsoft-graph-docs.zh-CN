---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c01ece2123df2ad3ac2d0832f750346530e90dc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096753"
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
graphClient.Communications().CallsById(&callId).Transfer().Post(options)


```