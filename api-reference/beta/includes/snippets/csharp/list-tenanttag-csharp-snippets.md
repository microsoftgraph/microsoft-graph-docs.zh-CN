---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eea6c7d33fbbcb25a2bd3a8dab0ac92da66cb66d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442363"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTags = await graphClient.TenantRelationships.ManagedTenants.TenantTags
    .Request()
    .GetAsync();

```