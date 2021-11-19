---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26141278e5da0d99cc7812e0bd7919c5740e45dd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082632"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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