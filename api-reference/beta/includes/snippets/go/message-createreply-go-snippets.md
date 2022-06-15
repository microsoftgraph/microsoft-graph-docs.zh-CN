---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 566b6897137696e7408dac8e415f0107c1d86e80
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "samanthab@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
name := "Samantha Booth"
    emailAddress.SetName(&name)
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "randiw@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
name := "Randi Welch"
    emailAddress.SetName(&name)
}
comment := "Samantha, Randi, would you name the group if the project is approved, please?"
requestBody.SetComment(&comment)
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReply(message-id).Post(requestBody)


```