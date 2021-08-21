---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 010937c99c5d66c65333b85fd977e6b514a57d035a3a030b634435170680a948
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162083"
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