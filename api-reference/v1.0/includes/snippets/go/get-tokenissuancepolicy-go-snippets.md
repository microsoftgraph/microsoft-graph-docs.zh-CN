---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f022960788929d74571dfb4fbf31036e40e1e61
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022888"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tokenIssuancePolicyId := "tokenIssuancePolicy-id"
result, err := graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Get(options)


```