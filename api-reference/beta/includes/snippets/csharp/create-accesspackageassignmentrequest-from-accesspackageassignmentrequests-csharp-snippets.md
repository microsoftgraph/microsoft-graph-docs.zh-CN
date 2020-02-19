---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c8ff1eab7c01d796b7e7b5c83ca7c488cbd4561
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992785"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequest
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