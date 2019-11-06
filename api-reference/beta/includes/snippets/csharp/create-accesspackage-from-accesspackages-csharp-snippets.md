---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61b526182bc2c0ec5c662b7a7482a20cc1997da1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackage = new AccessPackage
{
    CatalogId = "aa2f6514-3232-46e7-a08a-2411ad8d7128",
    DisplayName = "sales reps",
    Description = "outside sales representatives"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .Request()
    .AddAsync(accessPackage);

```