---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da9994cbee6cf937c6245544524050b523db7827
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098819"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "comment-value"
requestBody.SetComment(&comment)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
name := "name-value"
    emailAddress.SetName(&name)
address := "address-value"
    emailAddress.SetAddress(&address)
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Forward(message-id).Post(requestBody)


```