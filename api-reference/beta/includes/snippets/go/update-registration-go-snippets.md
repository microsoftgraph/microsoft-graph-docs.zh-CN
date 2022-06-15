---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5a6af5c112f13ac52d2c9d5b38e8c4dae912370
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098653"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMeetingRegistration()
subject := "Microsoft Ignite: Day 1"
requestBody.SetSubject(&subject)
startDateTime, err := time.Parse(time.RFC3339, "2021-11-02T08:00:00-08:00")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2021-11-02T15:45:00-08:00")
requestBody.SetEndDateTime(&endDateTime)
requestBody.SetSpeakers( []MeetingSpeaker {
    msgraphsdk.NewMeetingSpeaker(),
displayName := "Henry Ross"
    SetDisplayName(&displayName)
bio := "Chairman and Chief Executive Officer"
    SetBio(&bio)
    msgraphsdk.NewMeetingSpeaker(),
displayName := "Fred Ryan"
    SetDisplayName(&displayName)
bio := "CVP"
    SetBio(&bio)
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Patch(requestBody)


```