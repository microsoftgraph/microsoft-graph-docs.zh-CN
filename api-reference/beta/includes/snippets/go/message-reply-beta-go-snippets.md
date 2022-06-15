---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c1951cc62e05a649ae3ea3da2d2c17a9487e568
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098655"
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
comment := "Samantha, Randi, would you name the group please?"
requestBody.SetComment(&comment)
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Reply(message-id).Post(requestBody)


```