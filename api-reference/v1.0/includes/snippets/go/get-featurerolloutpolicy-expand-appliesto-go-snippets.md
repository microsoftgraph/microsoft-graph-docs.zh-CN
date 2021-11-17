---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b69d25915aeaccbcac1b8987f71bf3b0de559cc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993195"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.FeatureRolloutPolicyRequestBuilderGetQueryParameters{
    Expand: "appliesTo",
}
options := &msgraphsdk.FeatureRolloutPolicyRequestBuilderGetOptions{
    Q: requestParameters,
}
featureRolloutPolicyId := "featureRolloutPolicy-id"
result, err := graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Get(options)


```