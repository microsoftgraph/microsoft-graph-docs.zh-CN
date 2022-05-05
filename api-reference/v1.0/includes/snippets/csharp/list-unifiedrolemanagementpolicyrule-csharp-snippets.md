---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82a4211791329a4ec81a0b898de500e3272064ed
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204584"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rules = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].Rules
    .Request()
    .GetAsync();

```