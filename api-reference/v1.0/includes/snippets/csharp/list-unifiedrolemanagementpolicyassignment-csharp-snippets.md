---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5df72d9c67f1d25d83955eaa04691d78b18a79a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207357"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicyAssignments = await graphClient.Policies.RoleManagementPolicyAssignments
    .Request()
    .Filter("scopeId eq '/' and scopeType eq 'Directory'")
    .GetAsync();

```