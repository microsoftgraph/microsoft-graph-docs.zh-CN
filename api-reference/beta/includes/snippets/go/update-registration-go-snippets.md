---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfd1c25b9c42c942de7bdfe5b35cdbea5cba425b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011653"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.RegistrationRequestBuilderPatchOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Patch(options)


```