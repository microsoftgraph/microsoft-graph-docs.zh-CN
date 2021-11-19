---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63721abdfd9f05309af7ff0c51b4355828133657
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098356"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewThreatAssessmentRequest()
expectedAssessment := "block"
requestBody.SetExpectedAssessment(&expectedAssessment)
category := "spam"
requestBody.SetCategory(&category)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.mailAssessmentRequest",
    "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
    "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
}
options := &msgraphsdk.ThreatAssessmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.InformationProtection().ThreatAssessmentRequests().Post(options)


```