---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a542ec9e58a0cb438895a1b8f876e3a44d0f432
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411853"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

activityBasedTimeoutPolicyId := "activityBasedTimeoutPolicy-id"
result, err := graphClient.Policies().ActivityBasedTimeoutPoliciesById(&activityBasedTimeoutPolicyId).Delete(nil)


```