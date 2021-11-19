---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ff3c3f2e14635d4c4f47def3659fa8017ce48ab
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089638"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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