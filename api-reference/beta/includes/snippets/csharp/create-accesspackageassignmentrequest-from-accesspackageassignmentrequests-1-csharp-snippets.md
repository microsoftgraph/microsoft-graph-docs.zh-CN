---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c82ae80c249452f7c20285ca7bfea681d103503a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943226"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
    RequestType = "AdminAdd",
    AccessPackageAssignment = new AccessPackageAssignment
    {
        TargetId = "46184453-e63b-4f20-86c2-c557ed5d5df9",
        AssignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .AddAsync(accessPackageAssignmentRequest);

```