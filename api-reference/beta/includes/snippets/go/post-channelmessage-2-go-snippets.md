---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fe4d29a707fdc217d98e701f154e2c4c2c6588d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099119"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
createdDateTime, err := time.Parse(time.RFC3339, "2019-02-04T19:58:15.511Z")
requestBody.SetCreatedDateTime(&createdDateTime)
from := msgraphsdk.NewChatMessageFromIdentitySet()
requestBody.SetFrom(from)
from.SetAdditionalData(map[string]interface{}{
}
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "Hello World"
body.SetContent(&content)
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(options)


```