---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67fb22dd6e85a7254c5d6ac629ea690ca49e75de
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412469"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
defaultUserRolePermissions := msgraphsdk.NewDefaultUserRolePermissions()
requestBody.SetDefaultUserRolePermissions(defaultUserRolePermissions)
defaultUserRolePermissions.SetPermissionGrantPoliciesAssigned( []String {
    "managePermissionGrantsForSelf.microsoft-user-default-low",
}
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().AuthorizationPolicy().Patch(options)


```