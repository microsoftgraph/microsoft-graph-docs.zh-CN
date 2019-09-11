---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c12412ee40c2860455fac3c455fbb5982f7000e9
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignmentRequest = new PrivilegedRoleAssignmentRequest
{
    Duration = "2",
    Reason = "Activate the role for business purpose",
    TicketNumber = "234",
    TicketSystem = "system",
    Schedule = new GovernanceSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2018-02-08T02:35:17.903Z")
    },
    EvaluateOnly = false,
    Type = "UserAdd",
    AssignmentState = "Active",
    RoleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
};

await graphClient.PrivilegedRoleAssignmentRequests
    .Request()
    .AddAsync(privilegedRoleAssignmentRequest);

```