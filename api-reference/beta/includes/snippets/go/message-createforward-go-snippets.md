---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9cce17e6adfcf5f190be305551e5f0e6df38c4c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098811"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
isDeliveryReceiptRequested := true
message.SetIsDeliveryReceiptRequested(&isDeliveryReceiptRequested)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "danas@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
name := "Dana Swope"
    emailAddress.SetName(&name)
}
comment := "Dana, just want to make sure you get this; you'll need this if the project gets approved."
requestBody.SetComment(&comment)
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateForward(message-id).Post(requestBody)


```