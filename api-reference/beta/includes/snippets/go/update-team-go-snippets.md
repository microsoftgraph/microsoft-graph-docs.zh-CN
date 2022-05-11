---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fed70035816eb64be2bc99f6bc3be28a513b579e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326022"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeam()
isMembershipLimitedToOwners := true
requestBody.SetIsMembershipLimitedToOwners(&isMembershipLimitedToOwners)
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
discoverySettings := msgraphsdk.NewTeamDiscoverySettings()
requestBody.SetDiscoverySettings(discoverySettings)
showInTeamsSearchAndSuggestions := true
discoverySettings.SetShowInTeamsSearchAndSuggestions(&showInTeamsSearchAndSuggestions)
teamId := "team-id"
graphClient.TeamsById(&teamId).Patch(requestBody)


```