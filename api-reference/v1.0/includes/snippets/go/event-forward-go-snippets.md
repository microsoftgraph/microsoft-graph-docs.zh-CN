---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b8882e8525a5cd25dba47ba3901e6722db9b8ad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978953"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.Me().EventsById(&eventId).Forward().Post(options)


```