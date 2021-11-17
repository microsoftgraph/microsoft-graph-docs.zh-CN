---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3ec0ebe92e0e76472b721b6c8d0ae3c4b467911
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012144"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

featureRolloutPolicyId := "featureRolloutPolicy-id"
result, err := graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Get(options)


```