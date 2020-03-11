---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13d8d7407a58d7514aa42e7a3e884139a2cd37cb
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593481"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.HomeRealmDiscoveryPolicies["{id}"]
    .Request()
    .DeleteAsync();

```