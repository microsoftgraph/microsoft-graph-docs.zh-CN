---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ee783b40ce6039a799f8b1c520f2e63a9a011b6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983345"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AccessPackageResourceRolesRequestBuilderGetQueryParameters{
    Filter: "(originSystem%20eq%20'AadGroup'%20and%20accessPackageResource/id%20eq%20'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')",
    Expand: "accessPackageResource",
}
options := &msgraphsdk.AccessPackageResourceRolesRequestBuilderGetOptions{
    Q: requestParameters,
}
accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).AccessPackageResourceRoles().Get(options)


```