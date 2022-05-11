---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2c1e5ae46fa647f721abceff96b1c7141db1c60
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327454"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
result, err := graphClient.Me().OnlineMeetings().CreateOrGet().Post(requestBody)


```