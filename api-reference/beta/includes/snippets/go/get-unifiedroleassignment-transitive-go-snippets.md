---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e32cf90f768c632737f6f8172de9cc316f1a23c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338351"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TransitiveRoleAssignmentsRequestBuilderGetQueryParameters{
    Count: true,
    Filter: "principalId%20eq%20'2c7936bc-3517-40f3-8eda-4806637b6516'%20and%20roleDefinitionId%20eq%20'fe930be7-5e62-47db-91af-98c3a49a38b1'",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.TransitiveRoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.RoleManagement().Directory().TransitiveRoleAssignments().Get(options)


```