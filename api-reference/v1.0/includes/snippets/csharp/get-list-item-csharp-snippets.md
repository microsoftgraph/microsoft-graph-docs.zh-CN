---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ea7ba3db3bde8a349b06a1dba6d97c3b449d9ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "fields")
};

var listItem = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"]
    .Request( queryOptions )
    .GetAsync();

```