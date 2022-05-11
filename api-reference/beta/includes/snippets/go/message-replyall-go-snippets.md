---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 841e31941d6c814c5ce73560c6f2c79bb196e452
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328396"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetAttachments( []Attachment {
    msgraphsdk.NewAttachment(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
        "name": "guidelines.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=",
    }
}
comment := "Please take a look at the attached guidelines before you decide on the name."
requestBody.SetComment(&comment)
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).ReplyAll(message-id).Post(requestBody)


```