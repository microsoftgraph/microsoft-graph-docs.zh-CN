---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac670efd5f703e0c09c1b77b8d9b5060828f5b72
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminCustomers = await graphClient.TenantRelationships.DelegatedAdminCustomers
    .Request()
    .GetAsync();

```