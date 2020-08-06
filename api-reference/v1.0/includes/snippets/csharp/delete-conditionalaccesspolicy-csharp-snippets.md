---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4a6894052d762c94803499df0dae4e5482ce3a3
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.Policies["{id}"]
    .Request()
    .DeleteAsync();

```