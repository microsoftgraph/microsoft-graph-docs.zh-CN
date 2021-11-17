---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd4bd4211f15c98bd5e56ce8bcd1dd69b7f3d8ad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011765"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewMeetingRegistrationQuestion()
displayName := "What's your job position?"
requestBody.SetDisplayName(&displayName)
isRequired := false
requestBody.SetIsRequired(&isRequired)
answerInputType := "text"
requestBody.SetAnswerInputType(&answerInputType)
options := &msgraphsdk.CustomQuestionsRequestBuilderPostOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().CustomQuestions().Post(options)


```