---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff61ba16460a93b75775563020f804c917636de2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029854"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

activityBasedTimeoutPolicyId := "activityBasedTimeoutPolicy-id"
result, err := graphClient.Policies().ActivityBasedTimeoutPoliciesById(&activityBasedTimeoutPolicyId).Get(options)


```