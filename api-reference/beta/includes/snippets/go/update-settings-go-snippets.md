---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8eef609b58426f865538b5d04fc03aaac58d8597
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411648"
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
options := &msgraphsdk.SettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).Settings().Patch(options)


```