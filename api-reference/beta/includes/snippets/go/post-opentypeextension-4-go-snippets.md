---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4af21ce3c6e1326789f57813dec924d4e308cdea
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986003"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
post := msgraphsdk.NewPost()
requestBody.SetPost(post)
body := msgraphsdk.NewItemBody()
post.SetBody(body)
contentType := "html"
body.SetContentType(&contentType)
content := "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
body.SetContent(&content)
post.SetExtensions( []Extension {
    msgraphsdk.NewExtension(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.openTypeExtension",
        "extensionName": "Com.Contoso.HR",
        "companyName": "Contoso",
        "expirationDate": "2015-07-03T13:04:00.000Z",
        "topPicks":  []String {
            "Employees only",
            "Add spouse or guest",
            "Add family",
        }
    }
}
options := &msgraphsdk.ReplyRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
postId := "post-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).PostsById(&postId).Reply().Post(options)


```