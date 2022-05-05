---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b9a2f7d3bab51e5bc02f81a18fbea5418d05198
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicy = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"]
    .Request()
    .Expand("effectiveRules,rules")
    .GetAsync();

```