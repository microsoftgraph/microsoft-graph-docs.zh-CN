---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5736ab3c2b924da30f7284c1c3d7d3b8179774a1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicyCoverages = await graphClient.TenantRelationships.ManagedTenants.ConditionalAccessPolicyCoverages
    .Request()
    .GetAsync();

```