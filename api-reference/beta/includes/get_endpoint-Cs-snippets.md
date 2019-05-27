---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e95994522b0548f957101f3ff5be2408cb42847f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoint = await graphClient.Groups["{id}"].Endpoints["{id}"]
    .Request()
    .GetAsync();

```