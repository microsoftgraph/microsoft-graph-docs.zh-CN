---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6a26cc81dbbff363e8295e5c0ee401e32003bd4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087582"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.FeatureRolloutPolicyRequestBuilderGetQueryParameters{
    Expand: "appliesTo",
}
options := &msgraphsdk.FeatureRolloutPolicyRequestBuilderGetOptions{
    Q: requestParameters,
}
featureRolloutPolicyId := "featureRolloutPolicy-id"
result, err := graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Get(options)


```