---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a2db986c85e9f9347e5e2e20106e1852eedab03d
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest
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

await graphClient.PrivilegedAccess["azureResources"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```