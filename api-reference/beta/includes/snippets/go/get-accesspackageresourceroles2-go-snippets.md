---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fc31bccb8d449697d7cf8af6e386669ecdceef0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089192"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageResourceRolesRequestBuilderGetQueryParameters{
    Filter: "(originSystem%20eq%20'SharePointOnline'%20and%20accessPackageResource/id%20eq%20'53c71803-a0a8-4777-aecc-075de8ee3991')",
    Select: "displayName,originId",
}
options := &msgraphsdk.AccessPackageResourceRolesRequestBuilderGetOptions{
    Q: requestParameters,
}
accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).AccessPackageResourceRoles().Get(options)


```