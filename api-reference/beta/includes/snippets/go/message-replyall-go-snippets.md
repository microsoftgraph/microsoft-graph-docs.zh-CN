---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c54f0792bc70e4f349976ba00295683888e05c4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098744"
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
comment := "Please take a look at the attached guidelines before you decide on the name."
requestBody.SetComment(&comment)
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).ReplyAll(message-id).Post(requestBody)


```