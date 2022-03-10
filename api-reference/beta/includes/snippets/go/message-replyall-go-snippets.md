---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f2365ebd1fa5487abee3f820e0965380e2e0757
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412674"
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
options := &msgraphsdk.ReplyAllRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).ReplyAll(message-id).Post(options)


```