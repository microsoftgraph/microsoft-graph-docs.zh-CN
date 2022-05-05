---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95e92690ee451e45f2ee5806c612f03aefde35f6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208932"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
requestBody.SetSubject(nil)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "<attachment id="74d20c7f34aa4a7fb74e2b30004247c5"></attachment>"
body.SetContent(&content)
requestBody.SetAttachments( []ChatMessageAttachment {
    msgraphsdk.NewChatMessageAttachment(),
    SetAdditionalData(map[string]interface{}{
        "id": "74d20c7f34aa4a7fb74e2b30004247c5",
        "contentType": "application/vnd.microsoft.card.thumbnail",
        "contentUrl": nil,
        "content": "{
  "title": "This is an example of posting a card",
  "subtitle": "<h3>This is the subtitle</h3>",
  "text": "Here is some body text. <br>\r\nAnd a <a href=\"http://microsoft.com/\">hyperlink</a>. <br>\r\nAnd below that is some buttons:",
  "buttons": [
    {
      "type": "messageBack",
      "title": "Login to FakeBot",
      "text": "login",
      "displayText": "login",
      "value": "login"
    }
  ]
}",
        "name": nil,
        "thumbnailUrl": nil,
        "teamsAppId": "881b8843-fd91-49e5-9ac2-47ec497ffbe5",
    }
}
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(options)


```