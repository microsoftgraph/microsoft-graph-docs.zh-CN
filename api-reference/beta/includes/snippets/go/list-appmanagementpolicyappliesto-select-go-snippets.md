---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a8358d4491da671a54340cc1ae15b1ef97875a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326107"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppliesToRequestBuilderGetQueryParameters{
    Select: "id,appId,displayName,createdDateTime",
}
options := &msgraphsdk.AppliesToRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
appManagementPolicyId := "appManagementPolicy-id"
result, err := graphClient.Policies().AppManagementPoliciesById(&appManagementPolicyId).AppliesTo().GetWithRequestConfigurationAndResponseHandler(options, nil)


```