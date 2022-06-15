---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9237536205f01b71a02ad461e273a5b888118c3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098829"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
identity := msgraphsdk.NewIdentitySet()
    SetIdentity(identity)
user := msgraphsdk.NewIdentity()
    identity.SetUser(user)
id := "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
    user.SetId(&id)
upn := "test1@contoso.com"
    SetUpn(&upn)
}
result, err := graphClient.Me().OnlineMeetings().CreateOrGet().Post(requestBody)


```