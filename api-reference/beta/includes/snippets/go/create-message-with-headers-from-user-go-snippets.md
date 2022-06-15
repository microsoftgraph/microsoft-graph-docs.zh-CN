---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f063dfeedc194b07633d0b3c8de12f102eecbeeb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098821"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
subject := "9/8/2018: concert"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "HTML"
body.SetContentType(&contentType)
content := "The group represents Washington."
body.SetContent(&content)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "AlexW@contoso.OnMicrosoft.com"
    emailAddress.SetAddress(&address)
}
requestBody.SetInternetMessageHeaders( []InternetMessageHeader {
    msgraphsdk.NewInternetMessageHeader(),
name := "x-custom-header-group-name"
    SetName(&name)
value := "Washington"
    SetValue(&value)
    msgraphsdk.NewInternetMessageHeader(),
name := "x-custom-header-group-id"
    SetName(&name)
value := "WA001"
    SetValue(&value)
}
result, err := graphClient.Me().Messages().Post(requestBody)


```