---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f05bb17096e4c9e0c05b985c52d740962cff0464
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327327"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da",
}
featureRolloutPolicyId := "featureRolloutPolicy-id"
directoryObjectId := "directoryObject-id"
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).AppliesToById(&directoryObjectId).Post(requestBody)


```