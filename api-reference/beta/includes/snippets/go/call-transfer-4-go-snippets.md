---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 729ad0609726748727a90d3c8df593b9ce443e16
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327032"
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
callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer(call-id).Post(requestBody)


```