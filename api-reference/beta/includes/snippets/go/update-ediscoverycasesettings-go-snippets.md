---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ecf76aaf17b5de85605e480e46ca039dca57b68
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092418"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryCaseSettings()
redundancyDetection := msgraphsdk.NewRedundancyDetectionSettings()
requestBody.SetRedundancyDetection(redundancyDetection)
redundancyDetection.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.security.redundancyDetectionSettings",
}
topicModeling := msgraphsdk.NewTopicModelingSettings()
requestBody.SetTopicModeling(topicModeling)
topicModeling.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.security.topicModelingSettings",
}
ocr := msgraphsdk.NewOcrSettings()
requestBody.SetOcr(ocr)
ocr.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.security.ocrSettings",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.security.ediscoveryCaseSettings",
}
ediscoveryCaseId := "ediscoveryCase-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).Settings().Patch(requestBody)


```