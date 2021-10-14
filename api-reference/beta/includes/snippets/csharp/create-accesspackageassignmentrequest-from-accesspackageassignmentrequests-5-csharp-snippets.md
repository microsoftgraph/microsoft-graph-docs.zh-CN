---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1efebed85b9c4e959e3e24ff9da690f6273bed30
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60355186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
    RequestType = "AdminAdd",
    AccessPackageAssignment = new AccessPackageAssignment
    {
        Target = new AccessPackageSubject
        {
            Email = "user@contoso.com"
        },
        AssignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .AddAsync(accessPackageAssignmentRequest);

```