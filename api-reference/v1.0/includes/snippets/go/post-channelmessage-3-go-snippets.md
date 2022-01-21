---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a0bcb04231dda7b9ad35b3979df5db401527985
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104940"
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
id := "id-value"
user.SetId(&id)
displayName := "John Doe"
user.SetDisplayName(&displayName)
user.SetAdditionalData(map[string]interface{}{
    "userIdentityType": "aadUser",
}
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "<div><div>
<div><span><img height="250" src="../hostedContents/1/$value" width="176.2295081967213" style="vertical-align:bottom; width:176px; height:250px"></span>

</div>


</div>
</div>"
body.SetContent(&content)
requestBody.SetHostedContents( []ChatMessageHostedContent {
    msgraphsdk.NewChatMessageHostedContent(),
    SetAdditionalData(map[string]interface{}{
        "@microsoft.graph.temporaryId": "1",
        "contentBytes": "iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>",
        "contentType": "image/png",
    }
}
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Post(options)


```