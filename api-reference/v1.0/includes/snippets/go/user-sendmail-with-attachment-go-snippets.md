---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62729a91d936fc4a94d95159a6ebda811e394f14
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098704"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
subject := "Meet for lunch?"
message.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
message.SetBody(body)
contentType := "Text"
body.SetContentType(&contentType)
content := "The new cafeteria is open."
body.SetContent(&content)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "meganb@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
}
message.SetAttachments( []Attachment {
    msgraphsdk.NewAttachment(),
name := "attachment.txt"
    SetName(&name)
contentType := "text/plain"
    SetContentType(&contentType)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
        "contentBytes": "SGVsbG8gV29ybGQh",
    }
}
graphClient.Me().SendMail().Post(requestBody)


```