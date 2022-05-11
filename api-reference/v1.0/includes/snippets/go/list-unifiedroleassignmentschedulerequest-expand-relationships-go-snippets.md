---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70f828b2f62ee58ca33cb11edd42eb722a832952
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329040"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentScheduleRequestsRequestBuilderGetQueryParameters{
    Select: "principalId,action,roleDefinitionId",
    Expand: "roleDefinition,activatedUsing,principal,targetSchedule",
}
options := &msgraphsdk.RoleAssignmentScheduleRequestsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequests().GetWithRequestConfigurationAndResponseHandler(options, nil)


```