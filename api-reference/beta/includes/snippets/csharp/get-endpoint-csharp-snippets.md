---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e95994522b0548f957101f3ff5be2408cb42847f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622456"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoint = await graphClient.Groups["{id}"].Endpoints["{id}"]
    .Request()
    .GetAsync();

```