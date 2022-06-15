---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c74fb83f7a210d22f1ebcd4ea4a7c66d0fb196d7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098728"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "Hello World <at id="0">Jane Smith</at>"
body.SetContent(&content)
requestBody.SetMentions( []ChatMessageMention {
    msgraphsdk.NewChatMessageMention(),
id := int32(0)
    SetId(&id)
mentionText := "Jane Smith"
    SetMentionText(&mentionText)
mentioned := msgraphsdk.NewChatMessageMentionedIdentitySet()
    SetMentioned(mentioned)
user := msgraphsdk.NewIdentity()
    mentioned.SetUser(user)
displayName := "Jane Smith"
    user.SetDisplayName(&displayName)
id := "ef1c916a-3135-4417-ba27-8eb7bd084193"
    user.SetId(&id)
    user.SetAdditionalData(map[string]interface{}{
        "userIdentityType": "aadUser",
    }
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(requestBody)


```