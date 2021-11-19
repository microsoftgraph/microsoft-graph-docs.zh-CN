---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebbaf9bc2dd12cd260b43eab3ad38fa2a16aa13f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090559"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
post := msgraphsdk.NewPost()
requestBody.SetPost(post)
body := msgraphsdk.NewItemBody()
post.SetBody(body)
contentType := ""
body.SetContentType(&contentType)
content := "content-value"
body.SetContent(&content)
receivedDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
post.SetReceivedDateTime(&receivedDateTime)
hasAttachments := true
post.SetHasAttachments(&hasAttachments)
from := msgraphsdk.NewRecipient()
post.SetFrom(from)
emailAddress := msgraphsdk.NewEmailAddress()
from.SetEmailAddress(emailAddress)
name := "name-value"
emailAddress.SetName(&name)
address := "address-value"
emailAddress.SetAddress(&address)
sender := msgraphsdk.NewRecipient()
post.SetSender(sender)
emailAddress := msgraphsdk.NewEmailAddress()
sender.SetEmailAddress(emailAddress)
name := "name-value"
emailAddress.SetName(&name)
address := "address-value"
emailAddress.SetAddress(&address)
conversationThreadId := "conversationThreadId-value"
post.SetConversationThreadId(&conversationThreadId)
post.SetNewParticipants( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
conversationId := "conversationId-value"
post.SetConversationId(&conversationId)
createdDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
post.SetCreatedDateTime(&createdDateTime)
lastModifiedDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
post.SetLastModifiedDateTime(&lastModifiedDateTime)
changeKey := "changeKey-value"
post.SetChangeKey(&changeKey)
post.SetCategories( []String {
    "categories-value",
}
id := "id-value"
post.SetId(&id)
inReplyTo := msgraphsdk.NewPost()
post.SetInReplyTo(inReplyTo)
post.SetAttachments( []Attachment {
    msgraphsdk.NewAttachment(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": ,
        "isInline": true,
        "id": "id-value",
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