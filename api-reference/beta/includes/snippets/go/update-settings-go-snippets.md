---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef45868c9c6e6fe0ed58dffe2b09e0cfd2272b7c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCaseSettings()
redundancyDetection := msgraphsdk.NewRedundancyDetectionSettings()
requestBody.SetRedundancyDetection(redundancyDetection)
isEnabled := false
redundancyDetection.SetIsEnabled(&isEnabled)
similarityThreshold := int32(70)
redundancyDetection.SetSimilarityThreshold(&similarityThreshold)
minWords := int32(12)
redundancyDetection.SetMinWords(&minWords)
maxWords := int32(400000)
redundancyDetection.SetMaxWords(&maxWords)
topicModeling := msgraphsdk.NewTopicModelingSettings()
requestBody.SetTopicModeling(topicModeling)
isEnabled := false
topicModeling.SetIsEnabled(&isEnabled)
ignoreNumbers := false
topicModeling.SetIgnoreNumbers(&ignoreNumbers)
topicCount := int32(50)
topicModeling.SetTopicCount(&topicCount)
dynamicallyAdjustTopicCount := false
topicModeling.SetDynamicallyAdjustTopicCount(&dynamicallyAdjustTopicCount)
ocr := msgraphsdk.NewOcrSettings()
requestBody.SetOcr(ocr)
isEnabled := true
ocr.SetIsEnabled(&isEnabled)
maxImageSize := int32(12000)
ocr.SetMaxImageSize(&maxImageSize)
caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Settings().Patch(requestBody)


```