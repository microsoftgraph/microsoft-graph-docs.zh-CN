---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59a65f563e55d8cdd0c872f38be203669bec201d
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequestObject
{
    Action = "SelfActivate",
    PrincipalId = "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
    RoleDefinitionId = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    DirectoryScopeId = "/",
    Justification = "Need to update app roles for selected apps.",
    ScheduleInfo = new RequestSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2021-08-17T17:40:00Z"),
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