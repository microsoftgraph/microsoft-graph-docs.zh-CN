---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d54acc9950b75acb439ef952ee098d3abb4c213
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204506"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleManagementPolicyAssignmentId := "unifiedRoleManagementPolicyAssignment-id"
result, err := graphClient.Policies().RoleManagementPolicyAssignmentsById(&unifiedRoleManagementPolicyAssignmentId).Get(nil)


```