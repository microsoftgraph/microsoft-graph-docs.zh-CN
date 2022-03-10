---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 116547074170eed5c7151685523a5e4e7dc11441
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412040"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
comment := "Dana, hope you can make this meeting."
requestBody.SetComment(&comment)
options := &msgraphsdk.ForwardRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Forward(event-id).Post(options)


```