---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de044318577ce2dddda47b6e8285f342ee2e1687
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326217"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageRequestBuilderGetQueryParameters{
    Expand: "accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)",
}
options := &msgraphsdk.AccessPackageRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```