---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 061414a30208135468de5c017a03ebd3d5ea69fc
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098715"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPostRequestBody()
post := msgraphsdk.NewPost()
requestBody.SetPost(post)
body := msgraphsdk.NewItemBody()
post.SetBody(body)
contentType := "text"
body.SetContentType(&contentType)
content := "Which quarter does that file cover? See my attachment."
body.SetContent(&content)
post.SetAttachments( []Attachment {
    msgraphsdk.NewAttachment(),
name := "Another file as attachment"
    SetName(&name)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
        "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu",
    }
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Reply(group-id, conversationThread-id).Post(requestBody)


```