---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ff080334534d2fa75b83491454797ed093f776c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976530"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupLifecyclePolicyId := "groupLifecyclePolicy-id"
result, err := graphClient.GroupLifecyclePoliciesById(&groupLifecyclePolicyId).Get(options)


```