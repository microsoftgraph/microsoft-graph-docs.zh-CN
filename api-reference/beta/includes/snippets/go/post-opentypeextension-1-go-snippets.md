---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7960d7c601099ecd6f31b79f4b4e6363db335db5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
subject := "Annual review"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "HTML"
body.SetContentType(&contentType)
content := "You should be proud!"
body.SetContent(&content)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
requestBody.SetExtensions( []Extension {
    msgraphsdk.NewExtension(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.openTypeExtension",
        "extensionName": "Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "expirationDate": "2015-12-30T11:00:00.000Z",
        "dealValue": ,
    }
}
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Messages().Post(options)


```