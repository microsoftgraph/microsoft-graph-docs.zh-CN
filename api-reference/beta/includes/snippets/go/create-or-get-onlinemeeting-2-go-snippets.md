---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49d928cb1eb9cfe9d8a3b703983a91205db4701a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021706"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
chatInfo := msgraphsdk.NewChatInfo()
requestBody.SetChatInfo(chatInfo)
threadId := "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2"
chatInfo.SetThreadId(&threadId)
startDateTime, err := time.Parse(time.RFC3339, "2020-02-06T01:49:21.3524945+00:00")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2020-02-06T02:19:21.3524945+00:00")
requestBody.SetEndDateTime(&endDateTime)
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
subject := "Create a meeting with customId provided"
requestBody.SetSubject(&subject)
options := &msgraphsdk.CreateOrGetRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().OnlineMeetings().CreateOrGet().Post(options)


```