---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57a3ec1692653786dc81341ab758f938b4b6738b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilityScheduleRequest = new UnifiedRoleEligibilityScheduleRequestObject
{
    Action = UnifiedRoleScheduleRequestActions.AdminAssign,
    Justification = "Assign Attribute Assignment Admin eligibility to restricted user",
    RoleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    DirectoryScopeId = "/",
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b",
    ScheduleInfo = new RequestSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2022-04-10T00:00:00Z"),
        Expiration = new ExpirationPattern
        {
            Type = ExpirationPatternType.AfterDateTime,
            EndDateTime = DateTimeOffset.Parse("2024-04-10T00:00:00Z")
        }
    }
};

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests
    .Request()
    .AddAsync(unifiedRoleEligibilityScheduleRequest);

```