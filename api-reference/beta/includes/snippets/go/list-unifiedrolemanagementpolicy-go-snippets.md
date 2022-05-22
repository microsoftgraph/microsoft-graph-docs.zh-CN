---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6816783145dec9fc690bc4474d1cb2a2a1e9ea17
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629810"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleManagementPoliciesRequestBuilderGetQueryParameters{
    Filter: "scopeId%20eq%20'/'%20and%20scopeType%20eq%20'DirectoryRole'",
}
options := &msgraphsdk.RoleManagementPoliciesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Policies().RoleManagementPolicies().GetWithRequestConfigurationAndResponseHandler(options, nil)


```