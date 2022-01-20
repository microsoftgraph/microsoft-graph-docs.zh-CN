---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e49e838dfb11cf56caa0fa595e589d83d161df0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137645"
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
comment := "Samantha, Randi, would you name the group if the project is approved, please?"
requestBody.SetComment(&comment)
options := &msgraphsdk.CreateReplyRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReply().Post(options)


```