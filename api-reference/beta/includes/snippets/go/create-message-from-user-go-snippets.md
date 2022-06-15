---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c67597aa41deb43839bb20f9c78b7769aa82f37f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098822"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
subject := "Did you see last night's game?"
requestBody.SetSubject(&subject)
importance := "Low"
requestBody.SetImportance(&importance)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "HTML"
body.SetContentType(&contentType)
content := "They were <b>awesome</b>!"
body.SetContent(&content)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "AdeleV@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
}
result, err := graphClient.Me().Messages().Post(requestBody)


```