---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9190150a971162f2ceef9a4f78fac2d9f6d5f47
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315544"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleManagementPoliciesRequestBuilderGetQueryParameters{
    Filter: "scopeId%20eq%20'/'%20and%20scopeType%20eq%20'Directory'",
    Expand: "rules",
}
options := &msgraphsdk.RoleManagementPoliciesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Policies().RoleManagementPolicies().GetWithRequestConfigurationAndResponseHandler(options, nil)


```