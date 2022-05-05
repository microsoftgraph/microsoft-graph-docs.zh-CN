---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a14d177b6a1aad0cc0a49d789a6e72d8591ad3da
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "appScopeId%20eq%20'/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'",
    Expand: "principal",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.RoleManagement().EntitlementManagement().RoleAssignments().Get(options)


```