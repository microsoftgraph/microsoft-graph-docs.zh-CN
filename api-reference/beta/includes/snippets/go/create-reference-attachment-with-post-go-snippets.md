---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea39704d6f77aa2f674c219b4a4d58d625100f7e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098698"
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
content := "I attached a reference to a file on OneDrive."
body.SetContent(&content)
post.SetAttachments( []Attachment {
    msgraphsdk.NewAttachment(),
name := "Personal pictures"
    SetName(&name)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.referenceAttachment",
        "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
        "providerType": "oneDriveConsumer",
        "permission": "Edit",
        "isFolder": "True",
    }
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Reply(group-id, conversationThread-id).Post(requestBody)


```