---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abf57f6e554d634bd5fc3e569f1da4d19e53dabf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "fields")
};

var listItemVersion = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].Versions["{listItemVersion-id}"]
    .Request( queryOptions )
    .GetAsync();

```