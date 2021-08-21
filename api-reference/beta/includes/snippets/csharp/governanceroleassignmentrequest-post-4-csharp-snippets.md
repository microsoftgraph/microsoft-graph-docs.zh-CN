---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b0dc952dd384d623da941ef37e9833aa406e773309fd26da184001fcedd4a3d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162084"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequestObject
{
    RoleDefinitionId = "65bb4622-61f5-4f25-9d75-d0e20cf92019",
    ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    SubjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6",
    AssignmentState = "Eligible",
    Type = "AdminRemove"
};

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests
    .Request()
    .AddAsync(governanceRoleAssignmentRequest);

```