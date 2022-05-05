---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 923c685e23a63313e20ec6dd6a9c8aeda2f8b805
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203784"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageAssignmentRequestBuilderGetQueryParameters{
    Expand: "target",
}
options := &msgraphsdk.AccessPackageAssignmentRequestBuilderGetOptions{
    Q: requestParameters,
}
accessPackageAssignmentId := "accessPackageAssignment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentsById(&accessPackageAssignmentId).Get(options)


```