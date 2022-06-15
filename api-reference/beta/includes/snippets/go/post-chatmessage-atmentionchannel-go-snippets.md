---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dd1231bab45093c1b2c038c5c5c1f0d8e6e5d06
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098800"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "<div><div><at id="0">General</at>&nbsp;Hello there!</div></div>"
body.SetContent(&content)
requestBody.SetMentions( []ChatMessageMention {
    msgraphsdk.NewChatMessageMention(),
id := int32(0)
    SetId(&id)
mentionText := "General"
    SetMentionText(&mentionText)
mentioned := msgraphsdk.NewChatMessageMentionedIdentitySet()
    SetMentioned(mentioned)
conversation := msgraphsdk.NewTeamworkConversationIdentity()
    mentioned.SetConversation(conversation)
id := "19:0b50940236084d258c97b21bd01917b0@thread.skype"
    conversation.SetId(&id)
displayName := "General"
    conversation.SetDisplayName(&displayName)
conversationIdentityType := "channel"
    conversation.SetConversationIdentityType(&conversationIdentityType)
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(requestBody)


```