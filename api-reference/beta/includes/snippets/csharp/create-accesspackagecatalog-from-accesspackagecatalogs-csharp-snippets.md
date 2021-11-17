---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 747cc55d1003af48dc2336cd014d89e2d08bb758a68735b236398a0f952e57d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158636"
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