---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88d9971937ffc0997d61aa19013d22481ccabdf2
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528119"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var user = await graphClient.Me
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Expand("manager($levels=max;$select=id,displayName)")
    .Select("id,displayName")
    .GetAsync();

```