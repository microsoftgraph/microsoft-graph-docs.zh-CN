---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 78c28e2e90cc391ec9cd37cdca577da7749a4b55
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var items = await graphClient.Me.Drive.Items["{item-id}"]
    .Request( queryOptions )
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = items.Content;

```