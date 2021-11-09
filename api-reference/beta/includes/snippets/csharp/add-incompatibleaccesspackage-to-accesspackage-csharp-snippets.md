---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c294c9c486ee9d8c63a2615700e3fc467120f85
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageReference = new ReferenceRequestBody
{
    ODataId = "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleAccessPackages.References
    .Request()
    .AddAsync(accessPackageReference);

```