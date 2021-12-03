---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b10d03c23159caa1ad9d47355ed90ba5b477b9ed
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61289104"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
permissionGrantConditionSetId := "permissionGrantConditionSet-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).IncludesById(&permissionGrantConditionSetId).Delete(nil)


```