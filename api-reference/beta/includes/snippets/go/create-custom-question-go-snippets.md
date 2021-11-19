---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4309dcbb1fdcb8efb95f40df95380fb8707578bd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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