---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d33bf16dff49a16cde311ef723f43e02c1578a6baa43c338c6edd6d1b4b055e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequestObject
{
    RoleDefinitionId = "0e88fd18-50f5-4ee1-9104-01c3ed910065",
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    SubjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6",
    AssignmentState = "Eligible",
    Type = "AdminExtend",
    Reason = "extend role assignment",
    Schedule = new GovernanceSchedule
    {
        Type = "Once",
        StartDateTime = DateTimeOffset.Parse("2018-05-12T23:53:55.327Z"),
        EndDateTime = DateTimeOffset.Parse("2018-08-10T23:53:55.327Z")
    }
};

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```