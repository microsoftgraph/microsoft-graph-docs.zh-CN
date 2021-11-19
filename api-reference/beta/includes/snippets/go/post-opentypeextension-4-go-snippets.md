---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0d2818869549c416d786548ca409d51c3de1d5b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083467"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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