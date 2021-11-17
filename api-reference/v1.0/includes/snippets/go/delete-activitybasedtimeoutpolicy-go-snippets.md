---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89d5b9a4eef848ccc5ecb0bb0b4012f7d2d9c338
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029868"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

activityBasedTimeoutPolicyId := "activityBasedTimeoutPolicy-id"
graphClient.Policies().ActivityBasedTimeoutPoliciesById(&activityBasedTimeoutPolicyId).Delete(options)


```