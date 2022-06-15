---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 535a43e72d41ed88cba489c99cce81cc7ec9e9c6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098700"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "danas@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
name := "Dana Swope"
    emailAddress.SetName(&name)
}
comment := "Dana, hope you can make this meeting."
requestBody.SetComment(&comment)
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Forward(event-id).Post(requestBody)


```