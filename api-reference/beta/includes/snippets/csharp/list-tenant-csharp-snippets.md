---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fccf7dfbc2cb6c5901395ebda79be210c0832317
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440774"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenants = await graphClient.TenantRelationships.ManagedTenants.Tenants
    .Request()
    .GetAsync();

```