---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 736697026126dbb8dac776c543bd01188c0048e4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098402"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChannel()
displayName := "TestChannelModeration"
requestBody.SetDisplayName(&displayName)
description := "Test channel moderation."
requestBody.SetDescription(&description)
membershipType := "standard"
requestBody.SetMembershipType(&membershipType)
moderationSettings := msgraphsdk.NewChannelModerationSettings()
requestBody.SetModerationSettings(moderationSettings)
userNewMessageRestriction := "everyoneExceptGuests"
moderationSettings.SetUserNewMessageRestriction(&userNewMessageRestriction)
replyRestriction := "everyone"
moderationSettings.SetReplyRestriction(&replyRestriction)
allowNewMessageFromBots := true
moderationSettings.SetAllowNewMessageFromBots(&allowNewMessageFromBots)
allowNewMessageFromConnectors := true
moderationSettings.SetAllowNewMessageFromConnectors(&allowNewMessageFromConnectors)
options := &msgraphsdk.ChannelsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(options)


```