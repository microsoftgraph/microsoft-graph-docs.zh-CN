---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ac950d6e95a974c8222a88e81b4d331310b743c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023259"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
startDateTime, err := time.Parse(time.RFC3339, "2020-02-06T01:49:21.3524945+00:00")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2020-02-06T02:19:21.3524945+00:00")
requestBody.SetEndDateTime(&endDateTime)
subject := "Create a meeting with customId provided"
requestBody.SetSubject(&subject)
externalId := "7eb8263f-d0e0-4149-bb1c-1f0476083c56"
requestBody.SetExternalId(&externalId)
participants := msgraphsdk.NewMeetingParticipants()
requestBody.SetParticipants(participants)
participants.SetAttendees( []MeetingParticipantInfo {
    msgraphsdk.NewMeetingParticipantInfo(),
    SetAdditionalData(map[string]interface{}{
        "upn": "test1@contoso.com",
    }
}
options := &msgraphsdk.CreateOrGetRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().OnlineMeetings().CreateOrGet().Post(options)


```