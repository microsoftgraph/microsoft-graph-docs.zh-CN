---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 953c1e47e654fdbf22ccb09db4e321dcf7fdd043
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985097"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
    SetAdditionalData(map[string]interface{}{
    }
}
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Messages().Post(options)


```