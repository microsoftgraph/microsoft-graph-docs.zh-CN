---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 083b402a18e5c3affae630a9c682908a6faa7f2c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412359"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
permissionGrantConditionSetId := "permissionGrantConditionSet-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).ExcludesById(&permissionGrantConditionSetId).Delete(nil)


```