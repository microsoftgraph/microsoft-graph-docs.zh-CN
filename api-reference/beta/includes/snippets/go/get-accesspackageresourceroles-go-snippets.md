---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26306be89e3c8c2133c8f38d858c188076ff3b24
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087560"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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