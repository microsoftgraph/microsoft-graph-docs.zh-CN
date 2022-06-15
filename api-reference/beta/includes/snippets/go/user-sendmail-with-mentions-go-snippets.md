---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f84eaec6a567acbfd97d85405e935082de26dcaf
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098833"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
subject := "Project kickoff"
message.SetSubject(&subject)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
name := "Samantha Booth"
    emailAddress.SetName(&name)
address := "samanthab@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
}
message.SetMentions( []Mention {
    msgraphsdk.NewMention(),
mentioned := msgraphsdk.NewEmailAddress()
    SetMentioned(mentioned)
name := "Dana Swope"
    mentioned.SetName(&name)
address := "danas@contoso.onmicrosoft.com"
    mentioned.SetAddress(&address)
}
graphClient.Me().SendMail().Post(requestBody)


```