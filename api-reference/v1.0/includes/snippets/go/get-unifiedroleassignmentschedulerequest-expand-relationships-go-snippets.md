---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a70b31c18e4c9b2555fbc41dfc3bc499c7633477
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleAssignmentScheduleRequestRequestBuilderGetQueryParameters{
    Select: "principalId,action,roleDefinitionId",
    Expand: "roleDefinition,activatedUsing,principal,targetSchedule",
}
options := &msgraphsdk.UnifiedRoleAssignmentScheduleRequestRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleAssignmentScheduleRequestId := "unifiedRoleAssignmentScheduleRequest-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequestsById(&unifiedRoleAssignmentScheduleRequestId).Get(options)


```