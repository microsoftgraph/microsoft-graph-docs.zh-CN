---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2636ba1c77e921aa422ba3c8e627f197bcafed7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098578"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

featureRolloutPolicyId := "featureRolloutPolicy-id"
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Delete(options)


```