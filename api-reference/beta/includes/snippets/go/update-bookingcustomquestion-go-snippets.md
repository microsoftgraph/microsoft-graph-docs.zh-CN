---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c09cc74c81d6bf1d7ab3449fabdadbf3059cd57
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326392"
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
bookingBusinessId := "bookingBusiness-id"
bookingCustomQuestionId := "bookingCustomQuestion-id"
graphClient.BookingBusinessesById(&bookingBusinessId).CustomQuestionsById(&bookingCustomQuestionId).Patch(requestBody)


```