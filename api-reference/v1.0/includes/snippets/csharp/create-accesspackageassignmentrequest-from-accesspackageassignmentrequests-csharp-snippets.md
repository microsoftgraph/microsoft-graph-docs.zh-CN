---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 405f31c1c410e677f5c06c5cb2d3d04010ff6c65
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337920"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
    RequestType = AccessPackageRequestType.AdminRemove,
    Assignment = new AccessPackageAssignment
    {
        Id = "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests
    .Request()
    .AddAsync(accessPackageAssignmentRequest);

```