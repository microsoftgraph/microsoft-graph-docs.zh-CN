---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b214cf692bfd1f275ce6c5d5cecbf8455f23b88e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098693"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMeetingRegistrant()
firstName := "Lisa"
requestBody.SetFirstName(&firstName)
lastName := "Adkins"
requestBody.SetLastName(&lastName)
email := "lisa.adkins@contoso.com"
requestBody.SetEmail(&email)
requestBody.SetCustomQuestionAnswers( []CustomQuestionAnswer {
    msgraphsdk.NewCustomQuestionAnswer(),
    SetAdditionalData(map[string]interface{}{
        "questionId": "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=",
        "value": "No",
    }
    msgraphsdk.NewCustomQuestionAnswer(),
    SetAdditionalData(map[string]interface{}{
        "questionId": "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
        "value": "Internet",
    }
}
options := &msgraphsdk.RegistrantsRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
onlineMeetingId := "onlineMeeting-id"
result, err := graphClient.UsersById(&userId).OnlineMeetingsById(&onlineMeetingId).Registration().Registrants().Post(options)


```