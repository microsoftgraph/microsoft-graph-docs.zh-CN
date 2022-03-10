---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c38c20f4bdeea6a6f773538317bd8272ee6df3f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412468"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
defaultUserRolePermissions := msgraphsdk.NewDefaultUserRolePermissions()
requestBody.SetDefaultUserRolePermissions(defaultUserRolePermissions)
allowedToCreateApps := false
defaultUserRolePermissions.SetAllowedToCreateApps(&allowedToCreateApps)
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().AuthorizationPolicy().Patch(options)


```