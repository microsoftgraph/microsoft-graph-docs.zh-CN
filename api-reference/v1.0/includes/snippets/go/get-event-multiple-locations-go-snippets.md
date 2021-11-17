---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ba69dcfe541f2cbf78f79632fcb31f68788ab9f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016260"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,organizer,attendees,start,end,location,locations",
}
options := &msgraphsdk.EventRequestBuilderGetOptions{
    Q: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Get(options)


```