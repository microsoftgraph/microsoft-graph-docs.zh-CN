---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 068722586ade22f5c368e552c6209175e9502197
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var effectiveRules = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].EffectiveRules
    .Request()
    .GetAsync();

```