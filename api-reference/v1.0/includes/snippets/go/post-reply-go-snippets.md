---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22f520ef95b148c4782ebdffd98f47136ed1eda4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098778"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPostRequestBody()
post := msgraphsdk.NewPost()
requestBody.SetPost(post)
body := msgraphsdk.NewItemBody()
post.SetBody(body)
contentType := ""
body.SetContentType(&contentType)
content := "content-value"
body.SetContent(&content)
receivedDateTime, err := time.Parse(time.RFC3339, "datetime-value")
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
createdDateTime, err := time.Parse(time.RFC3339, "datetime-value")
post.SetCreatedDateTime(&createdDateTime)
lastModifiedDateTime, err := time.Parse(time.RFC3339, "datetime-value")
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
lastModifiedDateTime, err := time.Parse(time.RFC3339, "datetime-value")
    SetLastModifiedDateTime(&lastModifiedDateTime)
name := "name-value"
    SetName(&name)
contentType := "contentType-value"
    SetContentType(&contentType)
size := int32(99)
    SetSize(&size)
isInline := true
    SetIsInline(&isInline)
id := "id-value"
    SetId(&id)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
    }
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
postId := "post-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).PostsById(&postId).Reply(group-id, conversationThread-id, post-id).Post(requestBody)


```