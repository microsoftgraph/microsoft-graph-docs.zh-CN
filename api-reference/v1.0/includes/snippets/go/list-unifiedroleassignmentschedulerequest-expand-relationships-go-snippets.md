---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 163c80140230f4c7eddfb7862f190f9d2bd6ac91
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207240"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentScheduleRequestsRequestBuilderGetQueryParameters{
    Select: "principalId,action,roleDefinitionId",
    Expand: "roleDefinition,activatedUsing,principal,targetSchedule",
}
options := &msgraphsdk.RoleAssignmentScheduleRequestsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequests().Get(options)


```