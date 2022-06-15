---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cdc1db5a1ef4c7bc78d9304d6ca9813194bee42
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098684"
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
comment := "Dana, just want to make sure you get this."
requestBody.SetComment(&comment)
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Forward(message-id).Post(requestBody)


```