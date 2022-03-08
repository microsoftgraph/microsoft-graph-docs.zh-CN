---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ae1d35263e323b6c9d78a8f02c78ded236708f1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicy = new CrossTenantAccessPolicy
{
    DisplayName = "CrossTenantAccessPolicy"
};

await graphClient.Policies.CrossTenantAccessPolicy
    .Request()
    .UpdateAsync(crossTenantAccessPolicy);

```