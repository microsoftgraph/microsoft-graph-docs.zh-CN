---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0fae233525ac5da37679c3f2e8835957b07c21d
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566471"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = await graphClient.Identity.ConditionalAccess.NamedLocations["0854951d-5fc0-4eb1-b392-9b2c9d7949c2"]
    .Request()
    .GetAsync();

```