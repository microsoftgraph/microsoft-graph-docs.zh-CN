---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d3a012e390b6dba8e6337b1ad8c56359556b13c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411615"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermission()
requestBody.SetRoles( []String {
    "read",
}
options := &msgraphsdk.PermissionRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
permissionId := "permission-id"
result, err := graphClient.SitesById(&siteId).PermissionsById(&permissionId).Patch(options)


```