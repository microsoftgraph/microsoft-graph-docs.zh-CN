---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33eb1d30a516de5ff91e8407cba41c74578b893e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977480"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ThreatAssessmentRequestRequestBuilderGetQueryParameters{
    Expand: "results",
}
options := &msgraphsdk.ThreatAssessmentRequestRequestBuilderGetOptions{
    Q: requestParameters,
}
threatAssessmentRequestId := "threatAssessmentRequest-id"
result, err := graphClient.InformationProtection().ThreatAssessmentRequestsById(&threatAssessmentRequestId).Get(options)


```