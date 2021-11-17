---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8ac8eb3da0c3c02b4dc646d464f16b9c7aae45f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033487"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
unifiedRoleManagementPolicyRuleId := "unifiedRoleManagementPolicyRule-id"
result, err := graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).RulesById(&unifiedRoleManagementPolicyRuleId).Get(options)


```