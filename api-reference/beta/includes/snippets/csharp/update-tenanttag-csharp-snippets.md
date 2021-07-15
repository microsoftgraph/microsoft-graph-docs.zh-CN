---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85debec737ad73d078f6e0d77f4fe618c671bcae
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTag = new Microsoft.Graph.ManagedTenants.TenantTag
{
    DisplayName = "Onboarding",
    Description = "Tenants that we are currently onboarding"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .Request()
    .UpdateAsync(tenantTag);

```