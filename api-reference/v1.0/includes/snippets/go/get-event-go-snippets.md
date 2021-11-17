---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 420ef6d1ec710e1a7e944e88142c8ca0cad08f6b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016259"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees",
}
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.EventRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Get(options)


```