---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e58cd118e6558c9e8f46a9af79ab457d647d1c48
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = await graphClient.Identity.ConditionalAccess.Policies["{id}"]
    .Request()
    .GetAsync();

```