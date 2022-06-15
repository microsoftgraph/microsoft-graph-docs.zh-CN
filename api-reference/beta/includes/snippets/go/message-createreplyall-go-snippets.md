---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fa9ad931bd700d0a57d31898fa7030217a03ffd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098694"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetAttachments( []Attachment {
    msgraphsdk.NewAttachment(),
name := "guidelines.txt"
    SetName(&name)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=",
    }
}
comment := "if the project gets approved, please take a look at the attached guidelines before you decide on the name."
requestBody.SetComment(&comment)
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReplyAll(message-id).Post(requestBody)


```