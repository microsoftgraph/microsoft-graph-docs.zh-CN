---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 977c55f03001329eed79444cf2258b96a7890ba7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewThreatAssessmentRequest()
expectedAssessment := "block"
requestBody.SetExpectedAssessment(&expectedAssessment)
category := "malware"
requestBody.SetCategory(&category)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
    "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
    "contentData": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC.....",
}
options := &msgraphsdk.ThreatAssessmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.InformationProtection().ThreatAssessmentRequests().Post(options)


```