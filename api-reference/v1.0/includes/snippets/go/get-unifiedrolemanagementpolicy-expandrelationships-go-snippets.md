---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a782a0ff411af34bd4470e188ba397642aa47aa7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325880"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleManagementPolicyRequestBuilderGetQueryParameters{
    Expand: "effectiveRules,rules",
}
options := &msgraphsdk.UnifiedRoleManagementPolicyRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
result, err := graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```