---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 150f64f518e6c5cf2d04b82a638ca39d3b34e0d1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequestObject
{
    Action = UnifiedRoleScheduleRequestActions.SelfActivate,
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b",
    RoleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    DirectoryScopeId = "/",
    Justification = "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
    ScheduleInfo = new RequestSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2022-04-14T00:00:00Z"),
        Expiration = new ExpirationPattern
        {
            Type = ExpirationPatternType.AfterDuration,
            Duration = new Duration("PT5H")
        }
    },
    TicketInfo = new TicketInfo
    {
        TicketNumber = "CONTOSO:Normal-67890",
        TicketSystem = "MS Project"
    }
};

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .AddAsync(unifiedRoleAssignmentScheduleRequest);

```