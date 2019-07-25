---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 43e9656defd20f99a9b92b4a6c47e27fba764600
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "siteCollection,webUrl"),
    new QueryOption("filter", "siteCollection/root ne null")
};

var sites = await graphClient.Sites
    .Request( queryOptions )
    .Filter("siteCollection/root ne null")
    .GetAsync();

```