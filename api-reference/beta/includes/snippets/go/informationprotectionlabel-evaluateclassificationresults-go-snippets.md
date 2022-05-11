---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca161f9a207a7bfe629420891a1e2e698dd86951
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328284"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
options := &msgraphsdk.EvaluateClassificationResultsRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.InformationProtection().Policy().Labels().EvaluateClassificationResults().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```