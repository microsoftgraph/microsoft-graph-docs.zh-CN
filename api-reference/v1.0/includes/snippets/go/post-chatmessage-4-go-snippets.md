---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcf6037690300b0f64b246c2a3afa7f340466537
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "Here's the latest budget. <attachment id="153fa47d-18c9-4179-be08-9879815a9f90"></attachment>"
body.SetContent(&content)
requestBody.SetAttachments( []ChatMessageAttachment {
    msgraphsdk.NewChatMessageAttachment(),
id := "153fa47d-18c9-4179-be08-9879815a9f90"
    SetId(&id)
contentType := "reference"
    SetContentType(&contentType)
contentUrl := "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx"
    SetContentUrl(&contentUrl)
name := "Budget.docx"
    SetName(&name)
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(requestBody)


```