---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 931f27725a2706b506bc3c979da7b43448f6f5f5
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$skiptoken", "c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA=")
};

var chatMessage = await graphClient.Teams["{id}"].Channels["{id}"].Messages["delta"]
    .Request()
    .GetAsync();

```