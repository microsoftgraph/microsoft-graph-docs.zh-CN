---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac4ae5e02a4aa8da27d562d67cb217df10b0daed
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098804"
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
id := "74d20c7f34aa4a7fb74e2b30004247c5"
    SetId(&id)
contentType := "application/vnd.microsoft.card.thumbnail"
    SetContentType(&contentType)
    SetContentUrl(nil)
content := "{
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
}"
    SetContent(&content)
    SetName(nil)
    SetThumbnailUrl(nil)
teamsAppId := "881b8843-fd91-49e5-9ac2-47ec497ffbe5"
    SetTeamsAppId(&teamsAppId)
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(requestBody)


```