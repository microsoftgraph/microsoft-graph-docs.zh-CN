---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b911f3817f9ba9105bb7ce70b8b5b5b5f0254056
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034166"
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
comment := "Samantha, Randi, would you name the group if the project is approved, please?"
requestBody.SetComment(&comment)
options := &msgraphsdk.CreateReplyRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReply().Post(options)


```