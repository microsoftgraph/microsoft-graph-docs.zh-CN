---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fe29d332a9672b547f6be731dca8351351fb621
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095581"
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