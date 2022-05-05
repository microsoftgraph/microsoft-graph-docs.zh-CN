---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d42e5ae1d81b4ca3f0ec6c2d3eb7fe21652d7b8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminRelationship = await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"]
    .Request()
    .GetAsync();

```