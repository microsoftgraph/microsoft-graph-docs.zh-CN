---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcd3c94b24159b9cab751ff8e3e3d22897196047
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$skiptoken", "c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA=")
};

var chatMessage = await graphClient.Teams["{id}"].Channels["{id}"].Messages["delta"]
    .Request()
    .GetAsync();

```