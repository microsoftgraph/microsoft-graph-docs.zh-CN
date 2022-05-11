---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58dc91f04b00493de75227dfee7a55d267209a33
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicies = await graphClient.Policies.RoleManagementPolicies
    .Request()
    .Filter("scopeId eq '/' and scopeType eq 'Directory'")
    .Expand("rules")
    .GetAsync();

```