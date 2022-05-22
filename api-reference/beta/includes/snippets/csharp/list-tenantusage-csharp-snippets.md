---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0543b03580531f081763a285d71d686505a86605
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantUsage = await graphClient.TenantRelationships.ManagedTenants.TenantUsage
    .Request()
    .GetAsync();

```