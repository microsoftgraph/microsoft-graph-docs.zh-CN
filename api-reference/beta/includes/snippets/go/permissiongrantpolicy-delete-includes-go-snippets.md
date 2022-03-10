---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49e4d0b9f311e9226ef78a5b3f1d723381e8129e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412614"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
permissionGrantConditionSetId := "permissionGrantConditionSet-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).IncludesById(&permissionGrantConditionSetId).Delete(nil)


```