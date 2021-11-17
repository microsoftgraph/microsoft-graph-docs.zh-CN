---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dfeafeb367f767a6e4982c0fe65b012cea2ca35
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004785"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
contentInfo := msgraphsdk.NewContentInfo()
requestBody.SetContentInfo(contentInfo)
format := "default"
contentInfo.SetFormat(&format)
contentInfo.SetIdentifier(nil)
state := "rest"
contentInfo.SetState(&state)
contentInfo.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "state@odata.type": "#microsoft.graph.contentState",
}
requestBody.SetClassificationResults( []ClassificationResult {
    msgraphsdk.NewClassificationResult(),
    SetAdditionalData(map[string]interface{}{
        "sensitiveTypeId": "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
        "count": ,
        "confidenceLevel": ,
    }
}
headers := map[string]string{
    "User-Agent": "ContosoLOBApp/1.0"
}
options := &msgraphsdk.EvaluateClassificationResultsRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.InformationProtection().Policy().Labels().EvaluateClassificationResults().Post(options)


```