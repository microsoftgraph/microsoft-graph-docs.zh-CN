---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6cdd4145f3e46642b9c94c83e878bba1804d107
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignmentRequest = new PrivilegedRoleAssignmentRequestObject
{
    Duration = "2",
    Reason = "Activate the role for business purpose",
    TicketNumber = "234",
    TicketSystem = "system",
    Schedule = new GovernanceSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2018-02-08T02:35:17.903Z")
    },
    Type = "UserAdd",
    AssignmentState = "Active",
    RoleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
};

await graphClient.PrivilegedRoleAssignmentRequests
    .Request()
    .AddAsync(privilegedRoleAssignmentRequest);

```