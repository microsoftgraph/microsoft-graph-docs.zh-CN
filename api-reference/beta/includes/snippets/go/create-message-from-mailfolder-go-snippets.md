---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e87eb68e71d9d6ac8ee6053ce80c76ae5f117a7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102720"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
receivedDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
requestBody.SetReceivedDateTime(&receivedDateTime)
sentDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
requestBody.SetSentDateTime(&sentDateTime)
hasAttachments := true
requestBody.SetHasAttachments(&hasAttachments)
subject := "subject-value"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := ""
body.SetContentType(&contentType)
content := "content-value"
body.SetContent(&content)
bodyPreview := "bodyPreview-value"
requestBody.SetBodyPreview(&bodyPreview)
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Messages().Post(options)


```