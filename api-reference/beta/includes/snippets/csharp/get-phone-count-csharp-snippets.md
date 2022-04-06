---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6473234f526376015e39070db253b391a807d8c6
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var contacts = await graphClient.Contacts
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .GetAsync();

```