---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea1f67da7df329b8735fb85e6829854427705e2f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021964"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewMeetingRegistrationQuestion()
answerInputType := "radioButton"
requestBody.SetAnswerInputType(&answerInputType)
requestBody.SetAnswerOptions( []String {
    "Software Engineer",
    "Software Development Manager",
    "Product Manager",
    "Data scientist",
    "Other",
}
options := &msgraphsdk.MeetingRegistrationQuestionRequestBuilderPatchOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
meetingRegistrationQuestionId := "meetingRegistrationQuestion-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().CustomQuestionsById(&meetingRegistrationQuestionId).Patch(options)


```