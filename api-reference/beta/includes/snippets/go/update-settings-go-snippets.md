---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52341f9020ff30777e3ef7374253e6da14afd81b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015580"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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