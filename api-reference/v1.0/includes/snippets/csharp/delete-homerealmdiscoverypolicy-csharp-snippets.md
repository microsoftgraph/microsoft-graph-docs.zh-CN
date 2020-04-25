---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13d8d7407a58d7514aa42e7a3e884139a2cd37cb
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.HomeRealmDiscoveryPolicies["{id}"]
    .Request()
    .DeleteAsync();

```