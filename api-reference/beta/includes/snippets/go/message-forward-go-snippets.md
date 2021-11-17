---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15cb2ecc6cf8b65d83d6fa017ae010f2bc51804f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014579"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetAdditionalData(map[string]interface{}{
    "isDeliveryReceiptRequested": true,
    "toRecipients":  []Object {
    }
}
comment := "Dana, just want to make sure you get this."
requestBody.SetComment(&comment)
options := &msgraphsdk.ForwardRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Forward().Post(options)


```