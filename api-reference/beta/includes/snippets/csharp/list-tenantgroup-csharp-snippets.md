---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36797be1ca83b6885981bd6cdeab2dcefffab6bb946f4c7d16da317c6646bbf0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantGroups = await graphClient.TenantRelationships.ManagedTenants.TenantGroups
    .Request()
    .GetAsync();

```