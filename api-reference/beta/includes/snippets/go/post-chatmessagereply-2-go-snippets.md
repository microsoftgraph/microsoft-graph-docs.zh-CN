---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 932b318f44cfff89161282f502f7dc12b650921b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.RepliesRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).Replies().Post(options)


```