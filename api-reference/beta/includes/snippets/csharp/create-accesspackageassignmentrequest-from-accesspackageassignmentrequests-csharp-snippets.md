---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a1cc11b9fca3623e014379bed7c650475adbabd
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005833"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
    RequestType = "AdminRemove",
    AccessPackageAssignment = new AccessPackageAssignment
    {
        Id = "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .AddAsync(accessPackageAssignmentRequest);

```