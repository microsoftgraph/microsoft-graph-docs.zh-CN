---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 877e37b4cb7d051bf1c7a442765c66e5ee6ff401efab5c604f3c8ea783719cd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332933"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "name,lastModifiedDateTime"),
    new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))")
};

var list = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
    .Request( queryOptions )
    .GetAsync();

```