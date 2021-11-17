---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30431510b9b0243f0d3a79ed0a9a58a33b38b481
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewChatMessage()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "<div><div><at id="0">TestTag</at>&nbsp;Testing Tags</div></div>"
body.SetContent(&content)
requestBody.SetMentions( []ChatMessageMention {
    msgraphsdk.NewChatMessageMention(),
    SetAdditionalData(map[string]interface{}{
        "id": ,
        "mentionText": "TestTag",
    }
}
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(options)


```