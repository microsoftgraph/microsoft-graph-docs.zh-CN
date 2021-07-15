---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09a0591e7e4898bf1be89679abeb1ae087c0bb54
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActions = await graphClient.TenantRelationships.ManagedTenants.ManagementActions
    .Request()
    .GetAsync();

```