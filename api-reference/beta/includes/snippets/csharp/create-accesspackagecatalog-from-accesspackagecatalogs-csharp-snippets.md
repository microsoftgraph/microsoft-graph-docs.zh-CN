---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d541223635b523e6b1e38513f8d2f756cae12f35
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994213"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = new AccessPackageCatalog
{
    DisplayName = "sales",
    Description = "for employees working with sales and outside sales partners",
    IsExternallyVisible = true
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs
    .Request()
    .AddAsync(accessPackageCatalog);

```