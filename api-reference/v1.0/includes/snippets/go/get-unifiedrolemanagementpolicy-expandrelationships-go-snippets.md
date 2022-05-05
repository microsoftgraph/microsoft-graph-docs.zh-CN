---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e1d212070da3c53f06e8a813309356b972cd473
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleManagementPolicyRequestBuilderGetQueryParameters{
    Expand: "effectiveRules,rules",
}
options := &msgraphsdk.UnifiedRoleManagementPolicyRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
result, err := graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).Get(options)


```