---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 251b7335e11d6a147486cbb5bcd433c0b884e60d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985013"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
subject := "Project kickoff"
message.SetSubject(&subject)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
message.SetMentions( []Mention {
    msgraphsdk.NewMention(),
    SetAdditionalData(map[string]interface{}{
    }
}
options := &msgraphsdk.SendMailRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Me().SendMail().Post(options)


```