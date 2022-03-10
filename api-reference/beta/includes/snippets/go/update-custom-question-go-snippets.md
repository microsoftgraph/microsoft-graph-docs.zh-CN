---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf8bfb9db2896785db5622b273a33f7ee7e62488
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412369"
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
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().CustomQuestionsById(&meetingRegistrationQuestionId).Patch(options)


```