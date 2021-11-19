---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8469fd31fc52056d23a607400726978d49c24c5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099057"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeam()
memberSettings := msgraphsdk.NewTeamMemberSettings()
requestBody.SetMemberSettings(memberSettings)
allowCreateUpdateChannels := true
memberSettings.SetAllowCreateUpdateChannels(&allowCreateUpdateChannels)
messagingSettings := msgraphsdk.NewTeamMessagingSettings()
requestBody.SetMessagingSettings(messagingSettings)
allowUserEditMessages := true
messagingSettings.SetAllowUserEditMessages(&allowUserEditMessages)
allowUserDeleteMessages := true
messagingSettings.SetAllowUserDeleteMessages(&allowUserDeleteMessages)
funSettings := msgraphsdk.NewTeamFunSettings()
requestBody.SetFunSettings(funSettings)
allowGiphy := true
funSettings.SetAllowGiphy(&allowGiphy)
giphyContentRating := "strict"
funSettings.SetGiphyContentRating(&giphyContentRating)
options := &msgraphsdk.TeamRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Patch(options)


```