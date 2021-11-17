---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ee59bdc6bc3c573c43e7bb7a8d4a1987bc3be04
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012851"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
    SetAdditionalData(map[string]interface{}{
    }
}
message.SetInternetMessageHeaders( []InternetMessageHeader {
    msgraphsdk.NewInternetMessageHeader(),
    SetAdditionalData(map[string]interface{}{
        "name": "x-custom-header-group-name",
        "value": "Nevada",
    }
    msgraphsdk.NewInternetMessageHeader(),
    SetAdditionalData(map[string]interface{}{
        "name": "x-custom-header-group-id",
        "value": "NV001",
    }
}
options := &msgraphsdk.SendMailRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Me().SendMail().Post(options)


```