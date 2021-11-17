---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 825637f524065ccc8515a551d847073d26ac166b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978331"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderPostOptions{
    Body: requestBody,
}
featureRolloutPolicyId := "featureRolloutPolicy-id"
directoryObjectId := "directoryObject-id"
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).AppliesToById(&directoryObjectId).Post(options)


```