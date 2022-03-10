---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11c6f25f579e430c9cf0c1ecb509c18a6f6284cc
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411649"
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
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
        "name": "Another file as attachment",
        "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu",
    }
}
options := &msgraphsdk.ReplyRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Reply(group-id, conversationThread-id).Post(options)


```