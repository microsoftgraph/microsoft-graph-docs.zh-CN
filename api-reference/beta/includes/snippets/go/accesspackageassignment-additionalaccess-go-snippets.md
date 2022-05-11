---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c78cde2c1abded0537fe5b9db7d50aa10b2e290
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326209"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageAssignmentRequestBuilderGetQueryParameters{
    Expand: "target",
}
options := &msgraphsdk.AccessPackageAssignmentRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
accessPackageAssignmentId := "accessPackageAssignment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentsById(&accessPackageAssignmentId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```