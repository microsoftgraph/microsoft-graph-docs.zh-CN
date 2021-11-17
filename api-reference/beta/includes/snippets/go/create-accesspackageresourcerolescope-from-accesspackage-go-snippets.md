---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ae8cd3f386bcdde22291d5e00cb9fb436cff3e3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessPackageResourceRoleScope()
accessPackageResourceRole := msgraphsdk.NewAccessPackageResourceRole()
requestBody.SetAccessPackageResourceRole(accessPackageResourceRole)
accessPackageResourceRole.SetAdditionalData(map[string]interface{}{
    "originId": "Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
    "displayName": "Member",
    "originSystem": "AadGroup",
}
accessPackageResourceScope := msgraphsdk.NewAccessPackageResourceScope()
requestBody.SetAccessPackageResourceScope(accessPackageResourceScope)
accessPackageResourceScope.SetAdditionalData(map[string]interface{}{
    "originId": "b31fe1f1-3651-488f-bd9a-1711887fd4ca",
    "originSystem": "AadGroup",
}
options := &msgraphsdk.AccessPackageResourceRoleScopesRequestBuilderPostOptions{
    Body: requestBody,
}
accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).AccessPackageResourceRoleScopes().Post(options)


```