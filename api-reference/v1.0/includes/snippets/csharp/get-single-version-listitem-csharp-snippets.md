---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f87893900f981c6576fc13b4eb3cbf44df623844782f00ddd5b2e51ffddc0588
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409029"
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