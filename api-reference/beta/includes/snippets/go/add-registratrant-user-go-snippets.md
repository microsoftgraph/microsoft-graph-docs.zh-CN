---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0d51f8209a439f5ce08cdd0198d12940f4d42a7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980880"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewMeetingRegistrant()
firstName := "Frederick"
requestBody.SetFirstName(&firstName)
lastName := "Cormier"
requestBody.SetLastName(&lastName)
email := "frederick.cormier@contoso.com"
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