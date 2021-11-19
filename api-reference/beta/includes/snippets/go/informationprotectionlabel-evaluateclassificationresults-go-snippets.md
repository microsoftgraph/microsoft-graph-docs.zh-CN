---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08c85b1e4314753d25080df95ba2abb0e4cb03e4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103516"
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
options := &msgraphsdk.EvaluateClassificationResultsRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.InformationProtection().Policy().Labels().EvaluateClassificationResults().Post(options)


```