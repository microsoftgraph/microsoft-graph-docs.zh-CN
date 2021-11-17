---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11e63aa851451d11e58b03ebab7f3495baeb0a9b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009013"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOnlineMeeting()
startDateTime, err := time.Parse(time.RFC3339, "2019-07-12T14:30:34.2444915-07:00")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-07-12T15:00:34.2464912-07:00")
requestBody.SetEndDateTime(&endDateTime)
subject := "User Token Meeting"
requestBody.SetSubject(&subject)
options := &msgraphsdk.OnlineMeetingsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().OnlineMeetings().Post(options)


```