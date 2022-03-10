---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 106554cf7702e7a2b03629feaec56785478c3b36
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411698"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingCustomQuestion()
displayName := "What is your age?"
requestBody.SetDisplayName(&displayName)
answerInputType := "text"
requestBody.SetAnswerInputType(&answerInputType)
requestBody.SetAnswerOptions( []string {
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.bookingCustomQuestion",
}
options := &msgraphsdk.BookingCustomQuestionRequestBuilderPatchOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
bookingCustomQuestionId := "bookingCustomQuestion-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).CustomQuestionsById(&bookingCustomQuestionId).Patch(options)


```