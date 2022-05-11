---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab90e7a188b88f907438fbbfa9b95c326e6d1b60
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328707"
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
onlineMeetingId := "onlineMeeting-id"
meetingRegistrationQuestionId := "meetingRegistrationQuestion-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().CustomQuestionsById(&meetingRegistrationQuestionId).Patch(requestBody)


```