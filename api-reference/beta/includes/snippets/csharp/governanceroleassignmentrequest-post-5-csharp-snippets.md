---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b6d61afab2038589bb2691cc8ba183ab92cd091
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequestObject
{
    RoleDefinitionId = "70521f3e-3b95-4e51-b4d2-a2f485b02103",
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    SubjectId = "1566d11d-d2b6-444a-a8de-28698682c445",
    AssignmentState = "Eligible",
    Type = "AdminUpdate",
    Schedule = new GovernanceSchedule
    {
        Type = "Once",
        StartDateTime = DateTimeOffset.Parse("2018-03-08T05:42:45.317Z"),
        EndDateTime = DateTimeOffset.Parse("2018-06-05T05:42:31Z")
    }
};

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```