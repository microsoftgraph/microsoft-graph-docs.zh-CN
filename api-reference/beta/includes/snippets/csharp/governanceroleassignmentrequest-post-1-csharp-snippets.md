---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad9a1151ea4648847dcd1d916d5bfbc0b00060c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950771"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequestObject
{
    RoleDefinitionId = "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    AssignmentState = "Eligible",
    Type = "AdminAdd",
    Reason = "Assign an eligible role",
    Schedule = new GovernanceSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2018-05-12T23:37:43.356Z"),
        EndDateTime = DateTimeOffset.Parse("2018-11-08T23:37:43.356Z"),
        Type = "Once"
    }
};

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```