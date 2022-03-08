---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 411ba8fc2a6b0e7aad7dc20bd78194506fa8f812
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338348"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TransitiveRoleAssignmentsRequestBuilderGetQueryParameters{
    Count: true,
    Filter: "principalId%20eq%20'2c7936bc-3517-40f3-8eda-4806637b6516'%20and%20directoryScopeId%20eq%20'/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2'",
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