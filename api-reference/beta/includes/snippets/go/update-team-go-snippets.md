---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc3b5e3131d540c9391f8bc69038f7014cac6443
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977692"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.TeamRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Patch(options)


```