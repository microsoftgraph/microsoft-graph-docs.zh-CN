---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c43d4eedaf23de9937dfd310e45d41ace7fa502
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098805"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "<div><div><at id="0">GraphTesting</at>&nbsp;Hello team</div></div>"
body.SetContent(&content)
requestBody.SetMentions( []ChatMessageMention {
    msgraphsdk.NewChatMessageMention(),
id := int32(0)
    SetId(&id)
mentionText := "GraphTesting"
    SetMentionText(&mentionText)
mentioned := msgraphsdk.NewChatMessageMentionedIdentitySet()
    SetMentioned(mentioned)
conversation := msgraphsdk.NewTeamworkConversationIdentity()
    mentioned.SetConversation(conversation)
id := "68a3e365-f7d9-4a56-b499-24332a9cc572"
    conversation.SetId(&id)
displayName := "GraphTesting"
    conversation.SetDisplayName(&displayName)
conversationIdentityType := "team"
    conversation.SetConversationIdentityType(&conversationIdentityType)
}
requestBody.SetReactions( []ChatMessageReaction {
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(requestBody)


```