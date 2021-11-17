---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8b76094b625c6b7ab65d1161ed8e5cea410ff97
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003673"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

permissionGrantPolicyId := "permissionGrantPolicy-id"
permissionGrantConditionSetId := "permissionGrantConditionSet-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).IncludesById(&permissionGrantConditionSetId).Delete(options)


```