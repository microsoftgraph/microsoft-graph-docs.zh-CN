---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0910544c55d334c53dce18a4a3ce2c2571ff5cc2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412197"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
comment := "Samantha, Randi, would you name the group please?"
requestBody.SetComment(&comment)
options := &msgraphsdk.ReplyRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Reply(message-id).Post(options)


```