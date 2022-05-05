---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90152a1a14edad20dc9ae561ed1cf5b862a82d77
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicyAssignments = await graphClient.Policies.RoleManagementPolicyAssignments
    .Request()
    .Filter("scopeId eq '/' and scopeType eq 'DirectoryRole' and roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .Expand("policy($expand=rules)")
    .GetAsync();

```