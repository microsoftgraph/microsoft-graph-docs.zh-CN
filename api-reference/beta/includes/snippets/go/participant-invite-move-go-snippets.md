---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bd5755075db0e3c0800ad68ab35b00cad40bf5c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetParticipants( []InvitationParticipantInfo {
    msgraphsdk.NewInvitationParticipantInfo(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.invitationParticipantInfo",
        "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
        "participantId": "7d501bf1-5ee4-4605-ba92-0ae4513c611c",
    }
}
clientContext := "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
requestBody.SetClientContext(&clientContext)
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Participants().Invite(call-id).Post(requestBody)


```