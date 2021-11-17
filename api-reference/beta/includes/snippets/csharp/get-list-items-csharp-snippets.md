---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40242e2e2de7e4cb84e6cd9a8624f8dab459fdefc2c9b9040248741336a8d1cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103991"
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