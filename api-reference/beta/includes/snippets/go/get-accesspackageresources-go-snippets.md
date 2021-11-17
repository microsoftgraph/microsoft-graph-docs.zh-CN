---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ea15a6217bbaac7a25ea3c45ac287504b865b08
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983315"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AccessPackageResourcesRequestBuilderGetQueryParameters{
    Filter: "resourceType%20eq%20'Application'",
    Expand: "accessPackageResourceScopes",
}
options := &msgraphsdk.AccessPackageResourcesRequestBuilderGetOptions{
    Q: requestParameters,
}
accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).AccessPackageResources().Get(options)


```