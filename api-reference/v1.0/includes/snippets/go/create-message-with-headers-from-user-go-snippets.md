---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e239500138461af97064b9109d86f0a9faeedc2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090138"
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
    SetAdditionalData(map[string]interface{}{
    }
}
requestBody.SetInternetMessageHeaders( []InternetMessageHeader {
    msgraphsdk.NewInternetMessageHeader(),
    SetAdditionalData(map[string]interface{}{
        "name": "x-custom-header-group-name",
        "value": "Washington",
    }
    msgraphsdk.NewInternetMessageHeader(),
    SetAdditionalData(map[string]interface{}{
        "name": "x-custom-header-group-id",
        "value": "WA001",
    }
}
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Messages().Post(options)


```