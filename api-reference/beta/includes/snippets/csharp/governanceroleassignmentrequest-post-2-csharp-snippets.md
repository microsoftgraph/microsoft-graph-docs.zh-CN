---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53febd4de9bbe31e0e2ed987d2c75e0136cc28a8dcd5bdca8b04aa717a7b64fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequestObject
{
    RoleDefinitionId = "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    AssignmentState = "Active",
    Type = "UserAdd",
    Reason = "Activate the owner role",
    Schedule = new GovernanceSchedule
    {
        Type = "Once",
        StartDateTime = DateTimeOffset.Parse("2018-05-12T23:28:43.537Z"),
        Duration = new Duration("PT9H")
    },
    LinkedEligibleRoleAssignmentId = "e327f4be-42a0-47a2-8579-0a39b025b394"
};

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```