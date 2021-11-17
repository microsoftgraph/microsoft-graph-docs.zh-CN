---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b7dcc32108c90dc49bfb84bc02b9f339e9bf54bda59714bfbd2e169d5d404d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.ManagedTenants.Tenants["{managedTenants.tenant-id}"]
    .OffboardTenant()
    .Request()
    .PostAsync();

```