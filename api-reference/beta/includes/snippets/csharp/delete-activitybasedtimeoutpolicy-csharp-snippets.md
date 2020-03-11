---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d68c48222ad799d9f6e7549dfe0eee61efae57d7
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.ActivityBasedTimeoutPolicies["{id}"]
    .Request()
    .DeleteAsync();

```