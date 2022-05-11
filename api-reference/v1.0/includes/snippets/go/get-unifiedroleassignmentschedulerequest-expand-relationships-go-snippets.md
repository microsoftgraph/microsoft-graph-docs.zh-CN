---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9d45f29b75ba83a3ee8bc6a3b917374d5128bf5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleAssignmentScheduleRequestRequestBuilderGetQueryParameters{
    Select: "principalId,action,roleDefinitionId",
    Expand: "roleDefinition,activatedUsing,principal,targetSchedule",
}
options := &msgraphsdk.UnifiedRoleAssignmentScheduleRequestRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
unifiedRoleAssignmentScheduleRequestId := "unifiedRoleAssignmentScheduleRequest-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequestsById(&unifiedRoleAssignmentScheduleRequestId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```