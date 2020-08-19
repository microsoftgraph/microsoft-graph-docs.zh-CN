---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6e9c8b4536cd157f5aaec09e5611504ca0f800b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackage = new AccessPackage
{
    DisplayName = "Access Package New Name"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackageId}"]
    .Request()
    .UpdateAsync(accessPackage);

```