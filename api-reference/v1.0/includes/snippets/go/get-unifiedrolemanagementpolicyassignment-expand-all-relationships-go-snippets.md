---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6886a04e78ac71a921d9ff854566948fb7334ecc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleManagementPolicyAssignmentRequestBuilderGetQueryParameters{
    Expand: "policy($expand=rules)",
}
options := &msgraphsdk.UnifiedRoleManagementPolicyAssignmentRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
unifiedRoleManagementPolicyAssignmentId := "unifiedRoleManagementPolicyAssignment-id"
result, err := graphClient.Policies().RoleManagementPolicyAssignmentsById(&unifiedRoleManagementPolicyAssignmentId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```