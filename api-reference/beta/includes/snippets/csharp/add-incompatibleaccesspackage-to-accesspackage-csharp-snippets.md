---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e60cfc7dc6626014a07e925f2044055b80de1f1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageReference = new ReferenceRequestBody
{
    OdataId = "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleAccessPackages.References
    .Request()
    .AddAsync(accessPackageReference);

```