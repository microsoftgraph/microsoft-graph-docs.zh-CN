---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0093eedfa7701eafeeca93e3592f023604f2008b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088667"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
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
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.referenceAttachment",
        "name": "Personal pictures",
        "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
        "providerType": "oneDriveConsumer",
        "permission": "Edit",
        "isFolder": "True",
    }
}
options := &msgraphsdk.ReplyRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Reply().Post(options)


```