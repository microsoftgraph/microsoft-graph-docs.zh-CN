---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1f055a8508240567c704b845bee571205645011
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091634"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetAdditionalData(map[string]interface{}{
    "toRecipients":  []Object {
    }
}
comment := "Samantha, Randi, would you name the group please?"
requestBody.SetComment(&comment)
options := &msgraphsdk.ReplyRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Reply().Post(options)


```