---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec1f69b731720a6feedb209c27225b61f3ce18f7de30b8f57b2b9c6a8d7aac06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequestObject
{
    RoleDefinitionId = "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    ResourceId = "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    AssignmentState = "Active",
    Type = "UserRemove",
    Reason = "Deactivate the role",
    LinkedEligibleRoleAssignmentId = "cb8a533e-02d5-42ad-8499-916b1e4822ec"
};

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```