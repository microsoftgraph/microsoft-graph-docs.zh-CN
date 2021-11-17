---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a8e32eac66930e307c41c33c5315e1794a1ed017a2ac48ac2cbd952c76dabd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158662"
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