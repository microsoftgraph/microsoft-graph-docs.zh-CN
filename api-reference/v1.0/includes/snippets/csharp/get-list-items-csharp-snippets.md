---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 459800448ff7fced90890bf0b6951683f4dedcf3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "fields(select=Name,Color,Quantity)")
};

var items = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
    .Request( queryOptions )
    .GetAsync();

```