---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55ba1f662ed89e548952b606b0bc899373a1006a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082832"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,organizer,attendees,start,end,location,locations",
}
options := &msgraphsdk.EventRequestBuilderGetOptions{
    Q: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Get(options)


```