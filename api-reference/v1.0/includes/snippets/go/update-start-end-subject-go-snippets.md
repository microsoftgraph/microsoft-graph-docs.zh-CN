---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8b0cc86a7f3c8e7e8ba79789078786b26dd31f3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023225"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOnlineMeeting()
startDateTime, err := time.Parse(time.RFC3339, "2020-09-09T14:33:30.8546353-07:00")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2020-09-09T15:03:30.8566356-07:00")
requestBody.SetEndDateTime(&endDateTime)
subject := "Patch Meeting Subject"
requestBody.SetSubject(&subject)
options := &msgraphsdk.OnlineMeetingRequestBuilderPatchOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Patch(options)


```