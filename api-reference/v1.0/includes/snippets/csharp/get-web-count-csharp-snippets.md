---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aefb9dcbdb53356e465b0f463b32fe96e54789f2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var applications = await graphClient.Applications
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Web")
    .GetAsync();

```