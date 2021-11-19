---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4f7ef735b7363bf1d6d41081ad00addf6366b56
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103986"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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