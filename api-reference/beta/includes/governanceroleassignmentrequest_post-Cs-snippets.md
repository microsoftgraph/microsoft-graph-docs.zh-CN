---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a92a12cb93bb6f908913f77308aa98c2fb369db
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444935"
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
        StartDateTime = "2018-05-12T23:53:55.327Z",
        EndDateTime = "2018-08-10T23:53:55.327Z"
    }
};

await graphClient.PrivilegedAccess["azureResources"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```