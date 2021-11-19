---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3757515c14236c422005b5af4c0efa916ae7f38d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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