---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a56dd2ceca035fcd2d101cac90a8c9e65ad42e1e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var items = await graphClient.Drive.Items["{item-id}"]
    .Request( queryOptions )
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = items.Content;

```