---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ae407eca60eec0bb9cc5150facab4e21f101c7a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210174"
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
    .Filter("startswith(displayName, 'a')")
    .OrderBy("displayName")
    .GetAsync();

```