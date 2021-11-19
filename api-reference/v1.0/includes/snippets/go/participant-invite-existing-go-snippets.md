---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b3ed3e0b93778819bb236324196b7ad4d0f22b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094192"
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
    }
}
clientContext := "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.InviteRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Participants().Invite().Post(options)


```