---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d793d59b344a8b4e66186a4f07339dfe06bacccd
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTag = new Microsoft.Graph.ManagedTenants.TenantTag
{
    DisplayName = "Support",
    Description = "Tenants that have purchased extended support"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags
    .Request()
    .AddAsync(tenantTag);

```