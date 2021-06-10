---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d67eef891c4dd3dc498db8ec4bd75bbc3ee7e44
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
    RequestType = "UserAdd",
    AccessPackageAssignment = new AccessPackageAssignment
    {
        AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    Justification = "Need access to New Hire access package"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .AddAsync(accessPackageAssignmentRequest);

```