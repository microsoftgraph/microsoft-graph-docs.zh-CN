---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b78b0a18e059f5e424957ad5726a2f55a0457d70
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102920"
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
graphClient.SitesById(&siteId).PermissionsById(&permissionId).Patch(options)


```