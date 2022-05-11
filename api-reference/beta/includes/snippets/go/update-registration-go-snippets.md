---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06d149d4cff4dd183643ed61b20c9378985d0920
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326910"
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
    SetAdditionalData(map[string]interface{}{
        "displayName": "Henry Ross",
        "bio": "Chairman and Chief Executive Officer",
    }
    msgraphsdk.NewMeetingSpeaker(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Fred Ryan",
        "bio": "CVP",
    }
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Patch(requestBody)


```