---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ea6dc5292a7b00b91b2e10a4f95a8be9aeb1101
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207358"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters{
    Filter: "scopeId%20eq%20'/'%20and%20scopeType%20eq%20'DirectoryRole'%20and%20roleDefinitionId%20eq%20'62e90394-69f5-4237-9190-012177145e10'",
    Expand: "policy($expand=rules)",
}
options := &msgraphsdk.RoleManagementPolicyAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Policies().RoleManagementPolicyAssignments().Get(options)


```