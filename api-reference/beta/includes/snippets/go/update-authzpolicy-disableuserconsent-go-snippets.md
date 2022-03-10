---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88804b065c925a1727d7d5c7c329e62bc114e914
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412075"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
requestBody.SetPermissionGrantPolicyIdsAssignedToDefaultUserRole( []string {
}
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
authorizationPolicyId := "authorizationPolicy-id"
result, err := graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```