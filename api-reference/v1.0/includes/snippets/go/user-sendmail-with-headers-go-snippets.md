---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf1af6ff2d1ed5087c99ea37ec24a5296d00cdbd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
subject := "9/9/2018: concert"
message.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
message.SetBody(body)
contentType := "HTML"
body.SetContentType(&contentType)
content := "The group represents Nevada."
body.SetContent(&content)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "AlexW@contoso.OnMicrosoft.com"
    emailAddress.SetAddress(&address)
}
message.SetInternetMessageHeaders( []InternetMessageHeader {
    msgraphsdk.NewInternetMessageHeader(),
name := "x-custom-header-group-name"
    SetName(&name)
value := "Nevada"
    SetValue(&value)
    msgraphsdk.NewInternetMessageHeader(),
name := "x-custom-header-group-id"
    SetName(&name)
value := "NV001"
    SetValue(&value)
}
graphClient.Me().SendMail().Post(requestBody)


```