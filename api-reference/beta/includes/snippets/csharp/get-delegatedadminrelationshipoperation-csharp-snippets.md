---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05a013c55008d47da6b5eca75b51cff94322bb24
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204100"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminRelationshipOperation = await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].Operations["{delegatedAdminRelationshipOperation-id}"]
    .Request()
    .GetAsync();

```