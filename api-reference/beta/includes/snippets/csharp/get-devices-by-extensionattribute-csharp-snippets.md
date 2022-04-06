---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9261a20f5f4ed3d13bf3c0271becbd27904d5e06
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528077"
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
    .Filter("extensionAttributes/extensionAttribute1 eq 'BYOD-Device'")
    .GetAsync();

```