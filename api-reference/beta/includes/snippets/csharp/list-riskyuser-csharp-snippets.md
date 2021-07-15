---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a44cb3bd3f78697c1d9d11cbea981efaf2d0d28
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440808"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.TenantRelationships.ManagedTenants.RiskyUsers
    .Request()
    .GetAsync();

```