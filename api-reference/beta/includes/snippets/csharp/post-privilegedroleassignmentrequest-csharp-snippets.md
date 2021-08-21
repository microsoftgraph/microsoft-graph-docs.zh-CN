---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca4fe395d7a5c44f24a1887a98eb6a0dd1109a0c0a6e9657173c6406d0673329
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106872"
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