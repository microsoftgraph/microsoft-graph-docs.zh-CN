---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ade2e94131a232ebcf3974824bb11a00bcdf0612
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
isDeliveryReceiptRequested := true
message.SetIsDeliveryReceiptRequested(&isDeliveryReceiptRequested)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
comment := "Dana, just want to make sure you get this."
requestBody.SetComment(&comment)
options := &msgraphsdk.ForwardRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Forward(message-id).Post(options)


```