---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b2f92607a8b1e0ebadc6470266260827a0cc8ed
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicyAssignment = await graphClient.Policies.RoleManagementPolicyAssignments["{unifiedRoleManagementPolicyAssignment-id}"]
    .Request()
    .GetAsync();

```