---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83629738fcadcba26206e22aece568e4d8ddb8e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("search", "{query}")
};

var sites = await graphClient.Sites
    .Request( queryOptions )
    .GetAsync();

```