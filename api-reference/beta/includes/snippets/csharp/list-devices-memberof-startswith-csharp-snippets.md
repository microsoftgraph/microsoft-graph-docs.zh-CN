---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dc73afdbfdc0a4c0c2d13371d18b1b3621eb8be
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var group = await graphClient.Devices["{device-id}"].MemberOf
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName, 'A')")
    .OrderBy("displayName")
    .GetAsync();

```