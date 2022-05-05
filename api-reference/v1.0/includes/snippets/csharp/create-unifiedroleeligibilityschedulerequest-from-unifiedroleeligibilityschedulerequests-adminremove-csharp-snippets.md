---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da4c3544cb79b0f0e5103c2f2fa53495dc1794bc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilityScheduleRequest = new UnifiedRoleEligibilityScheduleRequestObject
{
    Action = "adminRemove",
    RoleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    DirectoryScopeId = "/",
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b"
};

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests
    .Request()
    .AddAsync(unifiedRoleEligibilityScheduleRequest);

```