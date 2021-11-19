---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b81954c1563c1f4bdaae2cfc47bc523863f01bee
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083266"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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