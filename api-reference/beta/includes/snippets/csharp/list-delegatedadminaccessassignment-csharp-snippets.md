---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77cf4558382744fada41b9f1f3dec35408c9639e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessAssignments = await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].AccessAssignments
    .Request()
    .GetAsync();

```