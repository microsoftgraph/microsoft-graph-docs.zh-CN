---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1c722663901eab47fcef36c9430e8cafe445fad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089191"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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