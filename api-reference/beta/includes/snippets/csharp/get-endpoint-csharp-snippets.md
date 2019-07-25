---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e95994522b0548f957101f3ff5be2408cb42847f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoint = await graphClient.Groups["{id}"].Endpoints["{id}"]
    .Request()
    .GetAsync();

```