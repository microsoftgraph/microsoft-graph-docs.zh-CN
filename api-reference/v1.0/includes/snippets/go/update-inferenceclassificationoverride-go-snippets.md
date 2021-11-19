---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c9adbcd96376df9d3446549d25def6fce8bd0ad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083091"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInferenceClassificationOverride()
classifyAs := "focused"
requestBody.SetClassifyAs(&classifyAs)
options := &msgraphsdk.InferenceClassificationOverrideRequestBuilderPatchOptions{
    Body: requestBody,
}
inferenceClassificationOverrideId := "inferenceClassificationOverride-id"
graphClient.Me().InferenceClassification().OverridesById(&inferenceClassificationOverrideId).Patch(options)


```