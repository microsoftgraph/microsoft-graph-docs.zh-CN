---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7ac85c41c52b536e73ee0afd3c80c619ba5a94b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095975"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChannel()
displayName := "UpdateChannelModeration"
requestBody.SetDisplayName(&displayName)
description := "Update channel moderation."
requestBody.SetDescription(&description)
moderationSettings := msgraphsdk.NewChannelModerationSettings()
requestBody.SetModerationSettings(moderationSettings)
userNewMessageRestriction := "moderators"
moderationSettings.SetUserNewMessageRestriction(&userNewMessageRestriction)
replyRestriction := "everyone"
moderationSettings.SetReplyRestriction(&replyRestriction)
allowNewMessageFromBots := true
moderationSettings.SetAllowNewMessageFromBots(&allowNewMessageFromBots)
allowNewMessageFromConnectors := true
moderationSettings.SetAllowNewMessageFromConnectors(&allowNewMessageFromConnectors)
options := &msgraphsdk.ChannelRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).Patch(options)


```