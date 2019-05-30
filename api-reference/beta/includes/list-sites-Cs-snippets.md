---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 43e9656defd20f99a9b92b4a6c47e27fba764600
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536972"
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