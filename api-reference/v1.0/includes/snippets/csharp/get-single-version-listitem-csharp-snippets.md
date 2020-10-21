---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6faaf3bfef4838755890c0c76541b7ff9e9012c6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "fields")
};

var listItemVersion = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Versions["{version-id}"]
    .Request( queryOptions )
    .GetAsync();

```