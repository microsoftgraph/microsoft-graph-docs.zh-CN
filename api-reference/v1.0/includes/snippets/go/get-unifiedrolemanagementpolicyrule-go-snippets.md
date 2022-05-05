---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7e4a0e3c9aba3ba5947a4190793881f6a6c2626
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204464"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
unifiedRoleManagementPolicyRuleId := "unifiedRoleManagementPolicyRule-id"
result, err := graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).RulesById(&unifiedRoleManagementPolicyRuleId).Get(nil)


```