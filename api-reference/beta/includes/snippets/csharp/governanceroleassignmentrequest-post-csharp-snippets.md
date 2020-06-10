---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a665c3743164006650f0e07566e2120a762ab39
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684814"
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

await graphClient.PrivilegedAccess["azureResources"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```