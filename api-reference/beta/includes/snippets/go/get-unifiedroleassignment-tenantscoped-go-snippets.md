---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffc2cd8a0160d9f82d2a9d588a84f626c6a03934
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325841"
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
options := &msgraphsdk.TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.RoleManagement().Directory().TransitiveRoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```