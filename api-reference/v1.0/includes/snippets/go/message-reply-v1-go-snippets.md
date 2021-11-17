---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc29aed7f03195b765bbcb75e2208baa0242a5df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029468"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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