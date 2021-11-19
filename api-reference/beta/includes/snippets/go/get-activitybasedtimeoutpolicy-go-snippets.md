---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 172137566e95ba535651bd7ea112e36123964aba
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087881"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

activityBasedTimeoutPolicyId := "activityBasedTimeoutPolicy-id"
result, err := graphClient.Policies().ActivityBasedTimeoutPoliciesById(&activityBasedTimeoutPolicyId).Get(options)


```