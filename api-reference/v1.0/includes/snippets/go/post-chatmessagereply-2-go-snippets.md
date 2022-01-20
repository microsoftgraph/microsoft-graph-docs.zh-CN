---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68b58b1f91f21e2feac80bb393090a891e13bd23
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088748"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
createdDateTime, err := time.Parse(time.RFC3339, "2019-02-04T19:58:15.511Z")
requestBody.SetCreatedDateTime(&createdDateTime)
from := msgraphsdk.NewChatMessageFromIdentitySet()
requestBody.SetFrom(from)
user := msgraphsdk.NewIdentity()
from.SetUser(user)
id := "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca"
user.SetId(&id)
displayName := "John Doe"
user.SetDisplayName(&displayName)
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