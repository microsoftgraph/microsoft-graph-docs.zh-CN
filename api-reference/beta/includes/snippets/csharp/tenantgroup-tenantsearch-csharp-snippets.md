---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06f8a2e91065fed5c9e19cfd198d757bb22b5febaaa3055402eb557a7424afe0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantId = "String";

await graphClient.TenantRelationships.ManagedTenants.TenantGroups
    .TenantSearch(tenantId)
    .Request()
    .PostAsync();

```