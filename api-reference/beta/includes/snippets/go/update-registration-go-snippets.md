---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37a2f39176b27af793982e4df6a67511bd4bd507
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092314"
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
options := &msgraphsdk.RegistrationRequestBuilderPatchOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Patch(options)


```