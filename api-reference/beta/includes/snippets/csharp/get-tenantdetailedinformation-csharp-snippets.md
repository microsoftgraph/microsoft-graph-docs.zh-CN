---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0527ab1f2fc8920bfea5b73bbe7e9bbbcdbb42ec
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantDetailedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsDetailedInformation["{managedTenants.tenantDetailedInformation-id}"]
    .Request()
    .GetAsync();

```