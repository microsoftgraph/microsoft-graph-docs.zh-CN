---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c7d3d518dfab1786698e738422b546e18707ca4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983738"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessPackageResourceRoleScope()
accessPackageResourceRole := msgraphsdk.NewAccessPackageResourceRole()
requestBody.SetAccessPackageResourceRole(accessPackageResourceRole)
accessPackageResourceRole.SetAdditionalData(map[string]interface{}{
    "originId": "4",
    "originSystem": "SharePointOnline",
}
accessPackageResourceScope := msgraphsdk.NewAccessPackageResourceScope()
requestBody.SetAccessPackageResourceScope(accessPackageResourceScope)
accessPackageResourceScope.SetAdditionalData(map[string]interface{}{
    "id": "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33",
    "originId": "https://microsoft.sharepoint.com/portals/Community",
    "originSystem": "SharePointOnline",
}
options := &msgraphsdk.AccessPackageResourceRoleScopesRequestBuilderPostOptions{
    Body: requestBody,
}
accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).AccessPackageResourceRoleScopes().Post(options)


```