---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c048829b25fde57f80c0fc2d482d2281bec62ae
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var group = await graphClient.Directory.DeletedItems
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Select("id,displayName,deletedDateTime")
    .OrderBy("deletedDateTime asc")
    .GetAsync();

```