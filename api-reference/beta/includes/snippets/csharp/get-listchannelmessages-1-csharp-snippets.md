---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7214254a829b7059adeace6a3d9fa9bfee4fe3f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("top", "3")
};

var messages = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request( queryOptions )
    .GetAsync();

```