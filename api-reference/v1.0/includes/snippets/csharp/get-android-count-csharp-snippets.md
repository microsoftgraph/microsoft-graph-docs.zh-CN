---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c111b802a5582517ca0d408a0cfece842f615c2f
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var devices = await graphClient.Devices
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Android")
    .GetAsync();

```