---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a66717c0b21f3a30dad1774463e0181a57988a11
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014539"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOnlineMeeting()
lobbyBypassSettings := msgraphsdk.NewLobbyBypassSettings()
requestBody.SetLobbyBypassSettings(lobbyBypassSettings)
isDialInBypassEnabled := true
lobbyBypassSettings.SetIsDialInBypassEnabled(&isDialInBypassEnabled)
options := &msgraphsdk.OnlineMeetingRequestBuilderPatchOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Patch(options)


```