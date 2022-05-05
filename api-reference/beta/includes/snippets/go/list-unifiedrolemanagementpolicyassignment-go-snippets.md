---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b040a92528cb9adfe77ce8455f7859abbc2707a8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220325"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters{
    Filter: "scopeId%20eq%20'/'%20and%20scopeType%20eq%20'Directory'",
}
options := &msgraphsdk.RoleManagementPolicyAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Policies().RoleManagementPolicyAssignments().Get(options)


```