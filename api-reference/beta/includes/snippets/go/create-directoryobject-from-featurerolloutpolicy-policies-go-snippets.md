---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf70268faac3c25ad4d49c86dabb2f4e2ad43838
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095179"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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