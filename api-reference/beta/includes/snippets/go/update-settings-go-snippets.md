---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 593ab5429448f9cc4f9a13ac60f86803e5076498
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224712"
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
graphClient.Compliance().Ediscovery().CasesById(&caseId).Settings().Patch(options)


```