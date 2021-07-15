---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3468ca9df81f14febe7e4d07a8df52e3c5fc0102
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.ManagedTenants.Tenants["{managedTenants.tenant-id}"]
    .OffboardTenant()
    .Request()
    .PostAsync();

```