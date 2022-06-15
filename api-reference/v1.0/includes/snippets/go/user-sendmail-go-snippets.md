---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07c07f22612cc9948cae299a9742f0e5b24a69a3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098702"
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
address := "fannyd@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
}
message.SetCcRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "danas@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
}
saveToSentItems := "false"
requestBody.SetSaveToSentItems(&saveToSentItems)
graphClient.Me().SendMail().Post(requestBody)


```