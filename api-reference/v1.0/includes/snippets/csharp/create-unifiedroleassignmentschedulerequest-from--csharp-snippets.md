---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90245bdc9643cea0a3fe7191da9d4a413437e73e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206798"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequestObject
{
    Action = UnifiedRoleScheduleRequestActions.AdminAssign,
    Justification = "Assign Groups Admin to IT Helpdesk group",
    RoleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    DirectoryScopeId = "/",
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b",
    ScheduleInfo = new RequestSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2022-04-10T00:00:00Z"),
        Expiration = new ExpirationPattern
        {
            Type = ExpirationPatternType.NoExpiration
        }
    }
};

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .AddAsync(unifiedRoleAssignmentScheduleRequest);

```