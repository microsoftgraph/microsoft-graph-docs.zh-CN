---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73284f3c3480aca0ba38814b3b1b7b58fd6ff277
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicyAssignment = await graphClient.Policies.RoleManagementPolicyAssignments["{unifiedRoleManagementPolicyAssignment-id}"]
    .Request()
    .Expand("policy($expand=rules)")
    .GetAsync();

```