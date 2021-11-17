---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85b7c56a3864f916ee2c6c2bfe627d6f9e054335
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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