---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a560571dbfe7f52271cedddd38e9c269737eecbf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083084"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
receivedDateTime, err := time.Parse(time.RFC3339, "datetime-value")
requestBody.SetReceivedDateTime(&receivedDateTime)
sentDateTime, err := time.Parse(time.RFC3339, "datetime-value")
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