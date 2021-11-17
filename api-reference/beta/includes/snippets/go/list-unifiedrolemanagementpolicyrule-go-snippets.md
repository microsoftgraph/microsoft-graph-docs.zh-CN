---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad03a3dcd41150d73b083e5f91f91701ede9118
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976831"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
result, err := graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).Rules().Get(options)


```