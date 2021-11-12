---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fdb1fc1492983719df37d3540c609b7f4e33fc5ed48025db6c8a2a450084c71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantIds = new List<String>()
{
    "String"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .UnassignTag(tenantIds)
    .Request()
    .PostAsync();

```