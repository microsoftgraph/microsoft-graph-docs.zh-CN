---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d6ce3e331bbea71f00ef088fdd03b9037261861
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327491"
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
graphClient.Me().SendMail().Post(requestBody)


```