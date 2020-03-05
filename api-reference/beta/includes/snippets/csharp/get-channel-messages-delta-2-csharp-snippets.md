---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5af4938b8565b3e421a82425a37eed6bc30014bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$skiptoken", "c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA=")
};

var delta = await graphClient.Teams["{id}"].Channels["{id}"].Messages
    .Delta()
    .Request()
    .GetAsync();

```