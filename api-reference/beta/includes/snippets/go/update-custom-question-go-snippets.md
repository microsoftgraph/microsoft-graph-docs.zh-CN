---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07faa859bbcfc598418952dea710080f2636b90d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098286"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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