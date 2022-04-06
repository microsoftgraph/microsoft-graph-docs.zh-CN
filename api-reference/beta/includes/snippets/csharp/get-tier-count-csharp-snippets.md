---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bc483b1f26173b3dbe4f21d18dba0f39f3c9d02
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var user = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:tier")
    .Select("displayName,id")
    .OrderBy("displayName")
    .GetAsync();

```